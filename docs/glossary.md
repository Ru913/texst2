# Glossary

## General Terms

- **Node.js**: A JavaScript runtime built on Chrome's V8 JavaScript engine, known for its event-driven, non-blocking I/O model.
- **Gulp**: A toolkit to automate time-consuming tasks in development workflows, such as linting, testing, and deployment.
- **UUID**: Universal Unique Identifier, used for generating unique ids.

## Project Specific Terms

- **DataOperation**: An abstract class defining operations within a DataSession. Methods include asynchronous processing and spawning child operations.
- **DataSession**: Manages the lifecycle of DataOperations, processing them asynchronously using a DataProvider.
- **DataSessionFactory**: Factory pattern implementation for creating and managing DataSession instances.
- **DataProvider**: Interface for data access mechanisms, abstracting the specific data storage or retrieval technologies.
- **DataOperationResult**: Represents the processing outcome of a DataOperation, including any child operations spawned.
- **DataOperationStage**: An enumeration defining the priority and order for processing DataOperation instances.
- **DataOperationAdjustment**: Used to adjust the priority order of operations being processed, depending on conditions.

## API Definitions

- **process(dataProvider, session, name)**: Method in DataOperation for processing the operation asynchronously.
- **startSession(callback, options)**: Method in DataSessionFactory to start a new session, managing its lifecycle.

## Configuration and Runtime

- **npm install @barchart/common-node-js -S**: Command to install the node module from NPM.

## Error Handling

- **Assert**: Used within classes like DataOperationStage to enforce certain conditions, such as argument types.

## Miscellaneous

- **MIT license**: The license under which the software is provided, allowing for free reuse of the source code.