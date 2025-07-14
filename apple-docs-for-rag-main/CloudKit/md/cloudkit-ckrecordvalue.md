

- CloudKit
-  CKRecordValue 

Type Alias

# CKRecordValue

A data type for objects that CloudKit stores on the server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+

``` source
typealias CKRecordValue = __CKRecordObjCValue
```

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

protocol CKRecordKeyValueSetting

A protocol for managing the key-value pairs of a CloudKit record.

