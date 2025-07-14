

- Foundation
- NSUbiquitousKeyValueStore
-  longLong(forKey:) 

Instance Method

# longLong(forKey:)

Returns the `long long` value associated with the specified key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func longLong(forKey aKey: String) -> Int64
```

## Parameters 

`aKey`  

A key in the key-value store.

## Return Value

The long long value associated with the specified key or `0` if the key was not found. If the key exists but does not contain a numerical value, this method returns `0`.

## See Also

### Related Documentation

func set(Int64, forKey: String)

Sets a `long long` value for the specified key in the key-value store.

### Getting Values

func array(forKey: String) -> [Any]?

Returns the array associated with the specified key.

func bool(forKey: String) -> Bool

Returns the Boolean value associated with the specified key.

func data(forKey: String) -> Data?

Returns the data object associated with the specified key.

func dictionary(forKey: String) -> [String : Any]?

Returns the dictionary object associated with the specified key.

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

func object(forKey: String) -> Any?

Returns the object associated with the specified key.

func string(forKey: String) -> String?

Returns the string associated with the specified key.

