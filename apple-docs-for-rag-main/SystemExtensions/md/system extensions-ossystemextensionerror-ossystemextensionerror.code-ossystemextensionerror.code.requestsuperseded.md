

- System Extensions
- OSSystemExtensionError
- OSSystemExtensionError.Code
-  OSSystemExtensionError.Code.requestSuperseded 

Case

# OSSystemExtensionError.Code.requestSuperseded

An error code that indicates the system extension request failed because the system already has a pending request for the same identifier.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
case requestSuperseded
```

## See Also

### Error Codes

case unknown

An error code that indicates an unknown error occurred.

case missingEntitlement

An error code that indicates the system extension lacks a required entitlement.

case unsupportedParentBundleLocation

An error code that indicates the extension’s parent app isn’t in a valid location for activation.

case extensionNotFound

An error code that indicates the manager can’t find the system extension.

case extensionMissingIdentifier

An error code that indicates the extension identifier is missing.

case duplicateExtensionIdentifer

An error code that indicates the extension identifier duplicates an existing identifier.

case unknownExtensionCategory

An error code that indicates the extension manager can’t recognize the extension’s category identifier.

case codeSignatureInvalid

An error code that indicates the extension’s signature is invalid.

case validationFailed

An error code that indicates the manager can’t validate the extension.

case forbiddenBySystemPolicy

An error code that indicates the system policy prohibits activating the system extension.

case requestCanceled

An error code that indicates the system extension manager request was canceled.

case authorizationRequired

An error code that indicates the system was unable to obtain the proper authorization.

