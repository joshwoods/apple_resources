

- CloudKit
- CKRecordKeyValueSetting
-  allKeys() 

Instance Method

# allKeys()

Returns an array of the record’s keys.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func allKeys() -> [String]
```

**Required**

## Return Value

An array of keys, or an empty array if the record doesn’t contain any keys.

## See Also

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

func changedKeys() -> [String]

Returns an array of keys with recent changes to their values.

**Required**

