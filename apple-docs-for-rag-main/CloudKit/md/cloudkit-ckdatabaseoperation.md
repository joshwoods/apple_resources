

- CloudKit
-  CKDatabaseOperation 

Class

# CKDatabaseOperation

The abstract base class for operations that act upon databases in CloudKit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKDatabaseOperation
```

## Overview

Database operations typically involve fetching and saving records and other database objects, as well as executing queries on the contents of the database. Use this class’s database property to tell the operation which database to use when you execute it. Don’t subclass this class or create instances of it. Instead, create instances of one of its concrete subclasses.

## Topics

### Accessing the Database

var database: CKDatabase?

The database that the operation uses.

## Relationships

### Inherits From

- CKOperation

### Inherited By

- CKFetchDatabaseChangesOperation
- CKFetchRecordChangesOperation
- CKFetchRecordZoneChangesOperation
- CKFetchRecordZonesOperation
- CKFetchRecordsOperation
- CKFetchSubscriptionsOperation
- CKFetchWebAuthTokenOperation
- CKModifyRecordZonesOperation
- CKModifyRecordsOperation
- CKModifySubscriptionsOperation
- CKQueryOperation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

