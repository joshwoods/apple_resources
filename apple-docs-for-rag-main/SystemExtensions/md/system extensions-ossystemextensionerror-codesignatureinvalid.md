

- System Extensions
- OSSystemExtensionError
-  codeSignatureInvalid 

Type Property

# codeSignatureInvalid

An error code that indicates the extension’s signature is invalid.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
static var codeSignatureInvalid: OSSystemExtensionError.Code { get }
```

## See Also

### Error Codes

enum Code

Error codes for system extensions.

static var unknown: OSSystemExtensionError.Code

An error code that indicates an unknown error occurred.

static var missingEntitlement: OSSystemExtensionError.Code

An error code that indicates the system extension lacks a required entitlement.

static var unsupportedParentBundleLocation: OSSystemExtensionError.Code

An error code that indicates the extension’s parent app isn’t in a valid location for activation.

static var extensionNotFound: OSSystemExtensionError.Code

An error code that indicates the manager can’t find the system extension.

static var extensionMissingIdentifier: OSSystemExtensionError.Code

An error code that indicates the extension identifier is missing.

static var duplicateExtensionIdentifer: OSSystemExtensionError.Code

An error code that indicates the extension identifier duplicates an existing identifier.

static var unknownExtensionCategory: OSSystemExtensionError.Code

An error code that indicates the extension manager can’t recognize the extension’s category identifier.

static var validationFailed: OSSystemExtensionError.Code

An error code that indicates the manager can’t validate the extension.

static var forbiddenBySystemPolicy: OSSystemExtensionError.Code

An error code that indicates the system policy prohibits activating the system extension.

static var requestCanceled: OSSystemExtensionError.Code

An error code that indicates the system extension manager request was canceled.

static var requestSuperseded: OSSystemExtensionError.Code

An error code that indicates the system extension request failed because the system already has a pending request for the same identifier.

static var authorizationRequired: OSSystemExtensionError.Code

An error code that indicates the system was unable to obtain the proper authorization.

