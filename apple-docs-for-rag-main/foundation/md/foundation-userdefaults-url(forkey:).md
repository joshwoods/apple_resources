

- Foundation
- UserDefaults
-  url(forKey:) 

Instance Method

# url(forKey:)

Returns the URL associated with the specified key.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func url(forKey defaultName: String) -> URL?
```

## Parameters 

`defaultName`  

A key in the current user’s defaults database.

## Return Value

The URL associated with the specified key. If the key doesn’t exist, this method returns `nil`.

## Discussion

This method retrieves the URL associated with a key with the following behavior:

1.  If the value for the key is an NSData object, the data object is used as the argument to unarchiveObject(with:). If the data object can be unarchived as an NSURL, the URL is returned. If the URL can’t be archived as an NSURL, `nil` is returned.

2.  If the value for this key is a file reference URL, the file reference URL is created, but its bookmark data isn’t resolved until the NSURL object is later used (for example, with init(contentsOfURL:)).

3.  If the value for the key is a string which begins with a tilde (~), the string is expanded using the expandingTildeInPath method, from which an NSURL with the `file:` scheme is created.

## See Also

### Related Documentation

func set(URL?, forKey: String)

Sets the value of the specified default key to the specified URL.

### Getting Default Values

func object(forKey: String) -> Any?

Returns the object associated with the specified key.

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

