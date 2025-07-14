

- Foundation
- Bundle
-  bundleURL 

Instance Property

# bundleURL

The full URL of the receiver’s bundle directory.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bundleURL: URL { get }
```

## See Also

### Getting Bundle Information

var bundlePath: String

The full pathname of the receiver’s bundle directory.

var bundleIdentifier: String?

The receiver’s bundle identifier.

var infoDictionary: [String : Any]?

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

func object(forInfoDictionaryKey: String) -> Any?

Returns the value associated with the specified key in the receiver’s information property list.

