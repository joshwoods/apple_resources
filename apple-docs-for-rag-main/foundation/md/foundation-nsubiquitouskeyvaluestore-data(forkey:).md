

- Foundation
- NSUbiquitousKeyValueStore
-  data(forKey:) 

Instance Method

# data(forKey:)

Returns the data object associated with the specified key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func data(forKey aKey: String) -> Data?
```

## Parameters 

`aKey`  

A key in the key-value store.

## Return Value

The data object associated with the specified key or `nil` if the key was not found or its value is not an NSData object.

## See Also

### Related Documentation

func set(Data?, forKey: String)

Sets a data object for the specified key in the key-value store.

### Getting Values

func array(forKey: String) -> [Any]?

Returns the array associated with the specified key.

func bool(forKey: String) -> Bool

Returns the Boolean value associated with the specified key.

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

