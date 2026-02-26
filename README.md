```markdown
# noona-hq/react-native-tcp

A React Native implementation of Node.js's net API for TCP communication.

## **Tech Stack**
- **Languages:** JavaScript, TypeScript
- **Frameworks:** React Native
- **Key Dependencies:** 
  - `react-native` (>=0.40.0)
  - `base64-js` (0.0.8)
  - `buffer` (^5.0.0)
  - `events` (^1.0.2)
  - `ip-regex` (^1.0.3)
  - `process` (^0.11.9)
  - `util` (^0.10.3)

## **Architecture / How it works**
- Implements a TCP server and client using React Native's native modules.
- Provides a JavaScript interface that mimics Node.js's `net` API for compatibility.
- Utilizes native Android and iOS code to handle low-level TCP socket operations.
- Exposes event-based APIs for handling connections, data streams, and errors.

## **Key interfaces / API**
- `TcpServer`: 
  - Methods: `listen`, `close`
  - Events: `connection`, `error`, `close`
- `TcpSocket`: 
  - Methods: `connect`, `write`, `end`, `destroy`
  - Events: `data`, `error`, `close`, `timeout`
- `TcpSockets`: 
  - Manages multiple socket instances and provides a unified interface for handling connections.

## **Dependencies**
- No direct dependencies on other Noona services. Relies on native modules for Android and iOS.
```