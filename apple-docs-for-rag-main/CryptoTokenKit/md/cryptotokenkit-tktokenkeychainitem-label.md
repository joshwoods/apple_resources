

- CryptoTokenKit
- TKTokenKeychainItem
-  label 

Instance Property

# label

The user-visible label for the keychain item.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var label: String? { get set }
```

## Discussion

This property is equivalent to the `kSecAttrLabel` attribute type.

## See Also

### Accessing Keychain Item Attributes

var objectID: TKToken.ObjectID

Returns the object ID used for keychain item identification.

var constraints: [NSNumber : Any]?

Access constraints for the keychain item, keyed by TKTokenOperation values wrapped in NSNumber objects.

