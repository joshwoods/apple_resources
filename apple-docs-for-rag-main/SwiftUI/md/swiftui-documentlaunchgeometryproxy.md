

- SwiftUI
-  DocumentLaunchGeometryProxy 

Structure

# DocumentLaunchGeometryProxy

A proxy for access to the frame of the scene and its title view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct DocumentLaunchGeometryProxy
```

## Topics

### Instance Properties

var frame: CGRect

Frame of the document launch interface.

var titleViewFrame: CGRect

Frame of the title view within the interface.

## See Also

### Configuring the document launch experience

struct DocumentGroupLaunchScene

A launch scene for document-based applications.

struct DocumentLaunchView

A view to present when launching document-related user experience.

struct DefaultDocumentGroupLaunchActions

The default actions for the document group launch scene and the document launch view.

struct NewDocumentButton

A button that creates and opens new documents.

protocol DocumentBaseBox

A Box that allows setting its Document base not requiring the caller to know the exact types of the box and its base.

