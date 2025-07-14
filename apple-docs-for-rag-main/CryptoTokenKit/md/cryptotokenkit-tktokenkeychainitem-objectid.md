

- CryptoTokenKit
- TKTokenKeychainItem
-  objectID 

Instance Property

# objectID

Returns the object ID used for keychain item identification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var objectID: TKToken.ObjectID { get }
```

## See Also

### Accessing Keychain Item Attributes

var label: String?

The user-visible label for the keychain item.

var constraints: [NSNumber : Any]?

Access constraints for the keychain item, keyed by TKTokenOperation values wrapped in NSNumber objects.

