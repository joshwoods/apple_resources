

- Foundation
- UserDefaults
-  stringArray(forKey:) 

Instance Method

# stringArray(forKey:)

Returns the array of strings associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func stringArray(forKey defaultName: String) -> [String]?
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The array of string objects, or `nil` if the specified default does not exist, the default does not contain an array, or the array does not contain strings.

## Discussion

The returned array and its contents are immutable, even if the values you originally set were mutable.

## See Also

### Related Documentation

func set(Any?, forKey: String)

Sets the value of the specified default key.

### Getting Default Values

func object(forKey: String) -> Any?

Returns the object associated with the specified key.

func url(forKey: String) -> URL?

Returns the URL associated with the specified key.

func array(forKey: String) -> [Any]?

Returns the array associated with the specified key.

func dictionary(forKey: String) -> [String : Any]?

Returns the dictionary object associated with the specified key.

func string(forKey: String) -> String?

Returns the string associated with the specified key.

func data(forKey: String) -> Data?

Returns the data object associated with the specified key.

func bool(forKey: String) -> Bool

Returns the Boolean value associated with the specified key.

func integer(forKey: String) -> Int

Returns the integer value associated with the specified key.

func float(forKey: String) -> Float

Returns the float value associated with the specified key.

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

func dictionaryRepresentation() -> [String : Any]

Returns a dictionary that contains a union of all key-value pairs in the domains in the search list.

