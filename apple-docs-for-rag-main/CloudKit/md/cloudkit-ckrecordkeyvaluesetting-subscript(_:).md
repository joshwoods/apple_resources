

- CloudKit
- CKRecordKeyValueSetting
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the object that the record stores for the specified key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
subscript(key: String) -> (any __CKRecordObjCValue)? { get set }
```

**Required** Default implementations provided.

## Parameters 

`key`  

The string that identifies a field in the record. A key must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces.

## Return Value

The object for the specified key, or `nil` if no such key exists in the record.

## Default Implementations

### CKRecordKeyValueSetting Implementations

subscript&lt;T>(CKRecord.FieldKey) -> T?

Accesses the value for the specified key in the record.

subscript(CKRecord.FieldKey) -> (any CKRecordValueProtocol)?

Accesses the value for the specified key in the record.

## See Also

### Accessing a Record’s Fields

func object(forKey: String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

**Required**

func setObject((any __CKRecordObjCValue)?, forKey: String)

Stores an object in the record using the specified key.

**Required**

func allKeys() -> [String]

Returns an array of the record’s keys.

**Required**

func changedKeys() -> [String]

Returns an array of keys with recent changes to their values.

**Required**

