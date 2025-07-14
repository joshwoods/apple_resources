

- SwiftUI
- DocumentConfiguration
-  fileURL 

Instance Property

# fileURL

A URL of an open document.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var fileURL: URL? { get }
```

## Discussion

If the document has never been saved, returns `nil`.

## See Also

### Getting configuration values

var isEditable: Bool

A Boolean value that indicates whether you can edit the document.

