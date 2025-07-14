

- Foundation
- UserDefaults
-  integer(forKey:) 

Instance Method

# integer(forKey:)

Returns the integer value associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func integer(forKey defaultName: String) -> Int
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The integer value associated with the specified key. If the specified key doesn’t exist, this method returns `0`.

## Discussion

This method automatically coerces certain values into equivalent integer values (if one can be determined). The Boolean value true becomes `1` and false becomes `0`. A floating point number becomes the greatest integer that’s less than that number (for example, `2.67` becomes `2`). A string that represents an integer becomes the equivalent integer (for example “123” becomes `123`).

## See Also

### Related Documentation

func set(Int, forKey: String)

Sets the value of the specified default key to the specified integer value.

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

func stringArray(forKey: String) -> [String]?

Returns the array of strings associated with the specified key.

func data(forKey: String) -> Data?

Returns the data object associated with the specified key.

func bool(forKey: String) -> Bool

Returns the Boolean value associated with the specified key.

func float(forKey: String) -> Float

Returns the float value associated with the specified key.

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

func dictionaryRepresentation() -> [String : Any]

Returns a dictionary that contains a union of all key-value pairs in the domains in the search list.

