

- UIKit
- UIPasteConfigurationSupporting
-  pasteConfiguration 

Instance Property

# pasteConfiguration

The paste configuration associated with the responder object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var pasteConfiguration: UIPasteConfiguration? { get set }
```

**Required**

## Discussion

If the responder object doesn’t have a paste configuration, `nil` is returned.

