

- Foundation
- UserDefaults
-  bool(forKey:) 

Instance Method

# bool(forKey:)

Returns the Boolean value associated with the specified key.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func bool(forKey defaultName: String) -> Bool
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The Boolean value associated with the specified key. If the specified key doesn’t exist, this method returns false.

## Discussion

This method automatically coerces certain “truthy” values—such as the strings “true”, “YES”, and “1”, and the numbers 1 and 1.0—to the Boolean value true. The same is true for certain “falsy” values—such as the strings “false”, “NO”, and “0”, and the numbers 0 and 0.0—which are automatically coerced to the Boolean value false.

## See Also

### Related Documentation

func set(Bool, forKey: String)

Sets the value of the specified default key to the specified Boolean value.

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

func integer(forKey: String) -> Int

Returns the integer value associated with the specified key.

func float(forKey: String) -> Float

Returns the float value associated with the specified key.

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

func dictionaryRepresentation() -> [String : Any]

Returns a dictionary that contains a union of all key-value pairs in the domains in the search list.

