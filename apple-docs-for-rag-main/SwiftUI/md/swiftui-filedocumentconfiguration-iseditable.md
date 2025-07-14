

- SwiftUI
- FileDocumentConfiguration
-  isEditable 

Instance Property

# isEditable

A Boolean that indicates whether you can edit the document.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var isEditable: Bool
```

## Discussion

This value is `false` if the document is in viewing mode, or if the file is not writable.

## See Also

### Getting document properties

var fileURL: URL?

The URL of the open file document.

