

- UIKit
-  UIDocumentPickerExtensionViewController Deprecated

Class

# UIDocumentPickerExtensionViewController

The principal class for the Document Picker View Controller extension.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
class UIDocumentPickerExtensionViewController
```

Deprecated

Use NSFileProviderExtension instead.

## Overview

The Document Picker View Controller extension can perform *import* and *export* operations on its own. If you want to support *open* and *move* operations, you must pair it with a File Provider extension.

When creating a Document Picker extension, you must subclass UIDocumentPickerExtensionViewController to provide the document picker’s user interface. Your subclass presents a list of available documents and destinations to the user. When the user makes a selection, you trigger the file transfer and pass the selected URL back to the host app.

For more information on creating Document Picker extensions, see Document Provider.

## Topics

### Managing the user interface

func dismissGrantingAccess(to: URL?)

Dismisses the document picker.

var documentPickerMode: UIDocumentPickerMode

The document picker’s file-transfer operation. (read-only)

var documentStorageURL: URL?

The root URL for documents provided by the corresponding File Provider extension. (read-only)

var originalURL: URL?

The URL of the file to be exported. (read-only)

func prepareForPresentation(in: UIDocumentPickerMode)

Performs any custom configuration of the document picker view controller.

var providerIdentifier: String

An identifier shared by this Document Picker extension and its corresponding File Provider extension. (read-only)

var validTypes: [String]?

An array of valid uniform type identifiers.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Document provider

class NSFileProviderExtension

The principal class for the nonreplicated File Provider extension.

