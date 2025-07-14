

- Foundation
- NSUbiquitousKeyValueStore
-  bool(forKey:) 

Instance Method

# bool(forKey:)

Returns the Boolean value associated with the specified key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func bool(forKey aKey: String) -> Bool
```

## Parameters 

`aKey`  

A key in the key-value store.

## Return Value

If a Boolean value is associated with the specified key, that value is returned. If the key was not found, this method returns false.

## See Also

### Related Documentation

func set(Bool, forKey: String)

Sets a Boolean value for the specified key in the key-value store.

### Getting Values

func array(forKey: String) -> [Any]?

Returns the array associated with the specified key.

func data(forKey: String) -> Data?

Returns the data object associated with the specified key.

func dictionary(forKey: String) -> [String : Any]?

Returns the dictionary object associated with the specified key.

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

func longLong(forKey: String) -> Int64

Returns the `long long` value associated with the specified key.

func object(forKey: String) -> Any?

Returns the object associated with the specified key.

func string(forKey: String) -> String?

Returns the string associated with the specified key.

