

- UIKit
- UIDocumentPickerViewController
-  shouldShowFileExtensions 

Instance Property

# shouldShowFileExtensions

A Boolean value that determines whether the browser always shows file extensions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var shouldShowFileExtensions: Bool { get set }
```

## Discussion

The default value is false.

Note

This property has no effect in Mac apps built with Mac Catalyst.

## See Also

### Configuring a document picker

var documentPickerMode: UIDocumentPickerMode

The type of file transfer operation that the document picker uses.

Deprecated

enum UIDocumentPickerMode

Modes that define the type of file transfer operation that the document picker uses.

Deprecated

