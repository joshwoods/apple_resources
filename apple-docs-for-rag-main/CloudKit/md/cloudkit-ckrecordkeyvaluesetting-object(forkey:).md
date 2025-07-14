

- CloudKit
- CKRecordKeyValueSetting
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the object that the record stores for the specified key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func object(forKey key: String) -> (any __CKRecordObjCValue)?
```

**Required**

## Parameters 

`key`  

The string that identifies a field in the record. A key must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces.

## Return Value

The object for the specified key, or `nil` if no such key exists in the record.

## See Also

### Accessing a Record’s Fields

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

