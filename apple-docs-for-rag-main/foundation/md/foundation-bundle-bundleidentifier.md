

- Foundation
- Bundle
-  bundleIdentifier 

Instance Property

# bundleIdentifier

The receiver’s bundle identifier.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var bundleIdentifier: String? { get }
```

## Discussion

The bundle identifier is defined by the `CFBundleIdentifier` key in the bundle’s information property list.

## See Also

### Getting Bundle Information

var bundleURL: URL

The full URL of the receiver’s bundle directory.

var bundlePath: String

The full pathname of the receiver’s bundle directory.

var infoDictionary: [String : Any]?

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

func object(forInfoDictionaryKey: String) -> Any?

Returns the value associated with the specified key in the receiver’s information property list.

