

- CloudKit
- CKRecord
-  setObject(\_:forKey:) 

Instance Method

# setObject(\_:forKey:)

Stores an object in the record using the specified key.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOSwatchOS 3.0+Swift 4.2+

``` source
func setObject(
    _ object: (any __CKRecordObjCValue)?,
    forKey key: CKRecord.FieldKey
)
```

## Parameters 

`object`  

The object to store using the specified key. It must be one of the data types in Supported Data Types. You receive an error if you use a data type that CloudKit doesn’t support. If you specify `nil`, CloudKit removes any object that the record associates with the key.

`key`  

The key to associate with `object`. Use this key to retrieve the value later. A key must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces. Avoid using a key that matches the name of any property of `CKRecord`.

## Discussion

If the specified key already exists in the record, CloudKit deletes its previous value and replaces it with the one in the `object` parameter. This change affects only the local copy of the record. You must save the record to the server again before the change becomes available to other clients.

If the type of the `object` parameter differs from the type of the object that’s on the server, you encounter an error when you attempt to save this record to the server. For example, if the current value is an NSString object, you receive an error if you change the value to an NSNumber object and save the record.

You access the fields of a `CKRecord` object the same way you access key-value pairs in a dictionary. The `CKRecord` class defines the objectForKey: and setObject:forKey: methods for getting and setting values. It also supports dictionary index notation. The following example shows how to use both techniques to set a `firstName` field and get a `lastName` field from a record:

```
// Equivalent ways to set a value.
let record = CKRecord(recordType: "Employee")
record.setObject(NSDate(), forKey: "hiredAt")
record["hiredAt"] = NSDate()
```

## See Also

### Accessing the Record’s Fields

func object(forKey: CKRecord.FieldKey) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

subscript(String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

subscript(CKRecord.FieldKey) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

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

