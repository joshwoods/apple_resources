

- Foundation
- Bundle
-  infoDictionary 

Instance Property

# infoDictionary

A dictionary, constructed from the bundle’s `Info.plist` file, that contains information about the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var infoDictionary: [String : Any]? { get }
```

## Discussion

If the bundle does not contain an `Info.plist` file, this dictionary contains only private keys that are used internally by the Bundle class. The Bundle class may add extra keys to this dictionary for its own use. Common keys for accessing the values of the dictionary are `CFBundleIdentifier`, `NSMainNibFile`, and `NSPrincipalClass`.

## See Also

### Related Documentation

var principalClass: AnyClass?

The bundle’s principal class.

### Getting Bundle Information

var bundleURL: URL

The full URL of the receiver’s bundle directory.

var bundlePath: String

The full pathname of the receiver’s bundle directory.

var bundleIdentifier: String?

The receiver’s bundle identifier.

func object(forInfoDictionaryKey: String) -> Any?

Returns the value associated with the specified key in the receiver’s information property list.

