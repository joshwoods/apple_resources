

- CloudKit
-  CKRecordKeyValueSetting 

Protocol

# CKRecordKeyValueSetting

A protocol for managing the key-value pairs of a CloudKit record.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
protocol CKRecordKeyValueSetting : NSObjectProtocol
```

## Topics

### Accessing a Record’s Fields

func object(forKey: String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

**Required**

subscript(String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

**Required** Default implementations provided.

func setObject((any __CKRecordObjCValue)?, forKey: String)

Stores an object in the record using the specified key.

**Required**

func allKeys() -> [String]

Returns an array of the record’s keys.

**Required**

func changedKeys() -> [String]

Returns an array of keys with recent changes to their values.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- CKRecord
- CKShare

## See Also

### Accessing the Record’s Fields

func object(forKey: CKRecord.FieldKey) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

subscript(String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

subscript(CKRecord.FieldKey) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

func setObject((any __CKRecordObjCValue)?, forKey: CKRecord.FieldKey)

Stores an object in the record using the specified key.

func allKeys() -> [CKRecord.FieldKey]

Returns an array of the record’s keys.

func changedKeys() -> [CKRecord.FieldKey]

Returns an array of keys with recent changes to their values.

struct CKRecordKeyValueIterator

An iterator of the record’s key-value pairs.

protocol CKRecordValueProtocol

A description of a CloudKit record value.

typealias CKRecordValue

A data type for objects that CloudKit stores on the server.

