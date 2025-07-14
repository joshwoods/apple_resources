

- CloudKit
- CKRecord
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the object that the record stores for the specified key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
func object(forKey key: CKRecord.FieldKey) -> (any __CKRecordObjCValue)?
```

## Parameters 

`key`  

The string that identifies a field in the record. A key must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces.

## Return Value

The object for the specified key, or `nil` if no such key exists in the record.

## Discussion

New records don’t contain any keys or values. Values are always one of the data types in Supported Data Types.

You access the fields of a `CKRecord` object the same way you access key-value pairs in a dictionary. The `CKRecord` class defines the objectForKey: and setObject:forKey: methods for getting and setting values. It also supports dictionary index notation. The following example shows how to use both techniques to set a `firstName` field and retrieve a `lastName` field from a record:

```
// Equivalent ways to get a value.
var hiredAt = record.object(forKey: "hiredAt")
hiredAt = record["hiredAt"]
```

## See Also

### Accessing the Record’s Fields

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

typealias CKRecordValue

A data type for objects that CloudKit stores on the server.

