# Database using C#

## Introduction
This project aims to create a custom database class library using C# that offers efficient storage and retrieval of arbitrary data. It provides functionality similar to SQLite but without its inefficiencies and performance degradation over time. The implemented database allows storing and managing records, particularly focusing on variable-length data, such as the example of storing information about cows.

## Features
- Efficient storage and retrieval of arbitrary data.
- Support for variable-length data records.
- Indexing for quick searching and retrieval of records based on specified criteria.
- Implementation of B-Tree data structure for indexing.
- Easy integration into any C# project as a DLL.
- Simple interface for CRUD operations on records.

## Design Overview
The database design consists of several components:
1. **Block Storage**: Provides low-level storage management using fixed-size blocks.
2. **Record Storage**: Builds on top of Block Storage to support variable-length records.
3. **Indexing**: Implements B-Tree structure for indexing records based on specified keys.
4. **Putting Things Together**: Integrates Record Storage and Indexing to create a complete database system.

## Implementation Details
- **Block Storage**: Handles storage of data in fixed-size blocks with metadata headers.
- **Record Storage**: Manages records by storing them as linked lists of blocks.
- **B-Tree (on disk)**: Implements B-Tree structure for indexing, with support for on-disk storage.
- **CowDatabase Implementation**: Utilizes Record Storage and Indexing to create a database for managing cow data.


## Feedback and Contributions
Feedback, bug reports, and contributions are welcome. Feel free to submit issues or pull requests on the GitHub repository.

