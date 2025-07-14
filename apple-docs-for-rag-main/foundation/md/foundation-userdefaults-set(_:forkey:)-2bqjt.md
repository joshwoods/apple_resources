

- Foundation
- UserDefaults
-  set(\_:forKey:) 

Instance Method

# set(\_:forKey:)

Sets the value of the specified default key to the specified URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func set(
    _ url: URL?,
    forKey defaultName: String
)
```

## Parameters 

`url`  

The URL to store in the defaults database.

`defaultName`  

The key with which to associate the value.

## Discussion

If `url` is a file URL, this method takes the absoluteURL, determines whether its path can be made relative to the user’s home directory, and if so, abbreviates it using the abbreviatingWithTildeInPath method.

If `url` isn’t a file URL, a data object is created by calling the archivedData(withRootObject:) method and passing `url` as the root object.

## See Also

### Related Documentation

func url(forKey: String) -> URL?

Returns the URL associated with the specified key.

### Setting Default Values

func set(Any?, forKey: String)

Sets the value of the specified default key.

func set(Float, forKey: String)

Sets the value of the specified default key to the specified float value.

func set(Double, forKey: String)

Sets the value of the specified default key to the double value.

func set(Int, forKey: String)

Sets the value of the specified default key to the specified integer value.

func set(Bool, forKey: String)

Sets the value of the specified default key to the specified Boolean value.

