

- CallKit
- CXStartCallAction
-  contactIdentifier 

Instance Property

# contactIdentifier

The identifier for the call recipient.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var contactIdentifier: String? { get set }
```

## Discussion

The identifier is displayed in the native call UI, and is typically the name of the call recipient.

If a caller corresponds to a CNContact object, set this to the value of the identifier property of the contact.

## See Also

### Accessing Action Attributes

var isVideo: Bool

A Boolean value that indicates whether the call is a video call.

var handle: CXHandle

The handle of the call recipient.

