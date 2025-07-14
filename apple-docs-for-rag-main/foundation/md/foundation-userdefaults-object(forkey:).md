

- Foundation
- UserDefaults
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns the object associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forKey defaultName: String) -> Any?
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The object associated with the specified key, or `nil` if the key was not found.

## Discussion

This method searches the domains included in the search list in the order in which they are listed and returns the object associated with the first occurrence of the specified default.

### Special Considerations

The returned object is immutable, even if the value you originally set was mutable.

## See Also

### Getting Default Values

func url(forKey: String) -> URL?

Returns the URL associated with the specified key.

func array(forKey: String) -> [Any]?

Returns the array associated with the specified key.

func dictionary(forKey: String) -> [String : Any]?

Returns the dictionary object associated with the specified key.

func string(forKey: String) -> String?

Returns the string associated with the specified key.

func stringArray(forKey: String) -> [String]?

Returns the array of strings associated with the specified key.

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

