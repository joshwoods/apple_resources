

- UIKit
-  UIDocumentPickerMode Deprecated

Enumeration

# UIDocumentPickerMode

Modes that define the type of file transfer operation that the document picker uses.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum UIDocumentPickerMode
```

## Topics

### Constants

case `import`

The document picker imports a file from outside the app’s sandbox.

case open

The document picker opens an external file outside the app’s sandbox.

case exportToService

The document picker exports a local file to a destination outside the app’s sandbox.

case moveToService

The document picker moves a local file outside the app’s sandbox and provides access to it as an external file.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring a document picker

var shouldShowFileExtensions: Bool

A Boolean value that determines whether the browser always shows file extensions.

var documentPickerMode: UIDocumentPickerMode

The type of file transfer operation that the document picker uses.

Deprecated

