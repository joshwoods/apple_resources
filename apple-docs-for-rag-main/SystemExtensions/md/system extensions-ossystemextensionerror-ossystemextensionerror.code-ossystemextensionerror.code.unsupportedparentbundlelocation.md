

- System Extensions
- OSSystemExtensionError
- OSSystemExtensionError.Code
-  OSSystemExtensionError.Code.unsupportedParentBundleLocation 

Case

# OSSystemExtensionError.Code.unsupportedParentBundleLocation

An error code that indicates the extension’s parent app isn’t in a valid location for activation.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
case unsupportedParentBundleLocation
```

## Discussion

The expected location of a driver extension is in the `Contents/Library/SystemExtensions` directory of a macOS app. The app itself must be in one of the system’s `Applications` directories.

## See Also

### Error Codes

case unknown

An error code that indicates an unknown error occurred.

case missingEntitlement

An error code that indicates the system extension lacks a required entitlement.

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

case requestSuperseded

An error code that indicates the system extension request failed because the system already has a pending request for the same identifier.

case authorizationRequired

An error code that indicates the system was unable to obtain the proper authorization.

