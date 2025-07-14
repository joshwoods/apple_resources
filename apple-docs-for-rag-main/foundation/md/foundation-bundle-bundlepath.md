

- Foundation
- Bundle
-  bundlePath 

Instance Property

# bundlePath

The full pathname of the receiver’s bundle directory.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bundlePath: String { get }
```

## See Also

### Getting Bundle Information

var bundleURL: URL

The full URL of the receiver’s bundle directory.

var bundleIdentifier: String?

The receiver’s bundle identifier.

var infoDictionary: [String : Any]?

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

func object(forInfoDictionaryKey: String) -> Any?

Returns the value associated with the specified key in the receiver’s information property list.

