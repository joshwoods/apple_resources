

- Foundation
- Bundle
-  object(forInfoDictionaryKey:) 

Instance Method

# object(forInfoDictionaryKey:)

Returns the value associated with the specified key in the receiver’s information property list.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forInfoDictionaryKey key: String) -> Any?
```

## Parameters 

`key`  

A key in the receiver’s property list.

## Return Value

The value associated with `key` in the receiver’s property list (`Info.plist`). The localized value of a key is returned when one is available.

## Discussion

Use of this method is preferred over other access methods because it returns the localized value of a key when one is available.

## See Also

### Getting Bundle Information

var bundleURL: URL

The full URL of the receiver’s bundle directory.

var bundlePath: String

The full pathname of the receiver’s bundle directory.

var bundleIdentifier: String?

The receiver’s bundle identifier.

var infoDictionary: [String : Any]?

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

