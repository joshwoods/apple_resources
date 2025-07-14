

- Foundation
- NSUbiquitousKeyValueStore
-  set(\_:forKey:) 

Instance Method

# set(\_:forKey:)

Sets a Boolean value for the specified key in the key-value store.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func set(
    _ value: Bool,
    forKey aKey: String
)
```

## Parameters 

`value`  

The Boolean value to store.

`aKey`  

The key under which to store the value. The length of this key must not exceed 64 bytes using UTF8 encoding.

## See Also

### Setting Values

func set([Any]?, forKey: String)

Sets an array object for the specified key in the key-value store.

func set(Data?, forKey: String)

Sets a data object for the specified key in the key-value store.

func set([String : Any]?, forKey: String)

Sets a dictionary object for the specified key in the key-value store.

func set(Double, forKey: String)

Sets a double value for the specified key in the key-value store.

func set(Int64, forKey: String)

Sets a `long long` value for the specified key in the key-value store.

func set(Any?, forKey: String)

Sets an object for the specified key in the key-value store.

func set(String?, forKey: String)

Sets a string object for the specified key in the key-value store.

