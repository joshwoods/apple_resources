

- CloudKit
- CKRecordKeyValueSetting
-  changedKeys() 

Instance Method

# changedKeys()

Returns an array of keys with recent changes to their values.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func changedKeys() -> [String]
```

**Required**

## Return Value

An array of keys with changed values since downloading or saving the record. If there aren’t any changed keys, this method returns an empty array.

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

func allKeys() -> [String]

Returns an array of the record’s keys.

**Required**

