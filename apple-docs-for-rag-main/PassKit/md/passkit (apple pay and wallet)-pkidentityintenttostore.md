

- PassKit (Apple Pay and Wallet)
-  PKIdentityIntentToStore 

Class

# PKIdentityIntentToStore

An object that represents your intention to store an identity element or values derived from an identity element.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
class PKIdentityIntentToStore
```

## Topics

### Creating a default intent

class func mayStore(days: Int) -> Self

An object that indicates your app may store a data element for the length of time you specify.

### Getting default intents

class var mayStore: PKIdentityIntentToStore

An object that indicates your app may store a data element for an indefinite length of time.

class var willNotStore: PKIdentityIntentToStore

An object that indicates your app won’t store a data element any longer than necessary to complete a request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Describing a document

class PKIdentityDriversLicenseDescriptor

An object for requesting information from a user’s driver’s license or equivalent document.

protocol PKIdentityDocumentDescriptor

A type that describes the structure and behavior of an identity document.

