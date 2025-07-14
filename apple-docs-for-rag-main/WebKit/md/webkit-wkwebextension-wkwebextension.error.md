

- WebKit
- WKWebExtension
-  WKWebExtension.Error 

Structure

# WKWebExtension.Error

Constants that indicate errors in the WKWebExtension domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Error
```

## Topics

### Type Properties

static var errorDomain: String

static var invalidArchive: WKWebExtension.Error.Code

Indicates that the archive file is invalid or corrupt.

static var invalidBackgroundPersistence: WKWebExtension.Error.Code

Indicates that the extension specified background persistence that was not compatible with the platform or features requested.

static var invalidDeclarativeNetRequestEntry: WKWebExtension.Error.Code

Indicates that an invalid declarative net request entry was encountered.

static var invalidManifest: WKWebExtension.Error.Code

Indicates that an invalid `manifest.json` was encountered.

static var invalidManifestEntry: WKWebExtension.Error.Code

Indicates that an invalid manifest entry was encountered.

static var invalidResourceCodeSignature: WKWebExtension.Error.Code

Indicates that a resource failed the bundle’s code signature checks.

static var resourceNotFound: WKWebExtension.Error.Code

Indicates that a specified resource was not found on disk.

static var unknown: WKWebExtension.Error.Code

Indicates that an unknown error occurred.

static var unsupportedManifestVersion: WKWebExtension.Error.Code

Indicates that the manifest version is not supported.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Structures

struct DataType

Constants for specifying data types for a WKWebExtension.DataRecord.

struct Permission

Constants for specifying permission in a WKWebExtensionContext.

struct TabChangedProperties

Constants the web extension controller and web extension context use to indicate tab changes.

