

- Foundation
- NSUbiquitousKeyValueStore
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the object associated with the specified key.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 9.0+

``` source
func object(forKey aKey: String) -> Any?
```

## Parameters 

`aKey`  

A key in the key-value store.

## Return Value

The object associated with the specified key or `nil` if the key was not found.

## Discussion

You can use this method to retrieve objects whose type you do not necessarily know from the key-value store. The object returned by this method is always one of the property list types: NSNumber, NSString, NSDate, NSData, NSArray, or NSDictionary.

## See Also

### Related Documentation

func set(Any?, forKey: String)

Sets an object for the specified key in the key-value store.

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

func longLong(forKey: String) -> Int64

Returns the `long long` value associated with the specified key.

func string(forKey: String) -> String?

Returns the string associated with the specified key.

