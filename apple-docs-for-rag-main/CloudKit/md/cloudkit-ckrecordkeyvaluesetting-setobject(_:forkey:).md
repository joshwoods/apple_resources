

- CloudKit
- CKRecordKeyValueSetting
-  setObject(\_:forKey:) 

Instance Method

# setObject(\_:forKey:)

Stores an object in the record using the specified key.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func setObject(
    _ object: (any __CKRecordObjCValue)?,
    forKey key: String
)
```

**Required**

## Parameters 

`object`  

The object to store using the specified key. It must be one of the data types in Supported Data Types. You receive an error if you use a data type that CloudKit doesn’t support. If you specify `nil`, CloudKit removes any object that the record associates with the key.

`key`  

The key to associate with `object`. Use this key to retrieve the value later. A key must consist of one or more alphanumeric characters and must start with a letter. CloudKit permits the use of underscores, but not spaces. Avoid using a key that matches the name of any property of `CKRecord`.

## See Also

### Accessing a Record’s Fields

func object(forKey: String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

**Required**

subscript(String) -> (any __CKRecordObjCValue)?

Returns the object that the record stores for the specified key.

**Required** Default implementations provided.

func allKeys() -> [String]

Returns an array of the record’s keys.

**Required**

func changedKeys() -> [String]

Returns an array of keys with recent changes to their values.

**Required**

