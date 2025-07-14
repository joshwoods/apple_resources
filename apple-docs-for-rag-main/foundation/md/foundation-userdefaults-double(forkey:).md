

- Foundation
- UserDefaults
-  double(forKey:) 

Instance Method

# double(forKey:)

Returns the double value associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func double(forKey defaultName: String) -> Double
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The double value associated with the specified key. If the key doesn’t exist, this method returns `0`.

## Discussion

This method automatically coerces certain values into equivalent double values (if one can be determined). The Boolean value true becomes `1.0` and false becomes `0.0`. An integer becomes the equivalent double (for example, `2` becomes `2.0`). A string that represents a floating point number becomes the equivalent double (for example “123.4” becomes `123.4`).

## See Also

### Related Documentation

func set(Double, forKey: String)

Sets the value of the specified default key to the double value.

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

func integer(forKey: String) -> Int

Returns the integer value associated with the specified key.

func float(forKey: String) -> Float

Returns the float value associated with the specified key.

func dictionaryRepresentation() -> [String : Any]

Returns a dictionary that contains a union of all key-value pairs in the domains in the search list.

