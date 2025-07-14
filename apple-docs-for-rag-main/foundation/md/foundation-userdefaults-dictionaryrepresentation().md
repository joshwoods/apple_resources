

- Foundation
- UserDefaults
-  dictionaryRepresentation() 

Instance Method

# dictionaryRepresentation()

Returns a dictionary that contains a union of all key-value pairs in the domains in the search list.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dictionaryRepresentation() -> [String : Any]
```

## Return Value

A dictionary containing the keys. The keys are names of defaults and the value corresponding to each key is a property list object (NSData, NSString, NSNumber, NSDate, NSArray, or NSDictionary).

## Discussion

As with object(forKey:), key-value pairs in domains that are earlier in the search list take precedence. The combined result does not preserve information about which domain each entry came from.

## See Also

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

func double(forKey: String) -> Double

Returns the double value associated with the specified key.

