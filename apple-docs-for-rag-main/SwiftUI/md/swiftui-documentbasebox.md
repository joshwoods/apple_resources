

- SwiftUI
-  DocumentBaseBox 

Protocol

# DocumentBaseBox

A Box that allows setting its Document base not requiring the caller to know the exact types of the box and its base.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
protocol DocumentBaseBox : AnyObject
```

## Topics

### Associated Types

associatedtype Document

The underlying document type.

**Required**

### Instance Properties

var base: Self.Document?

Updates the underlying document to a new value.

**Required**

## See Also

### Configuring the document launch experience

struct DocumentGroupLaunchScene

A launch scene for document-based applications.

struct DocumentLaunchView

A view to present when launching document-related user experience.

struct DocumentLaunchGeometryProxy

A proxy for access to the frame of the scene and its title view.

struct DefaultDocumentGroupLaunchActions

The default actions for the document group launch scene and the document launch view.

struct NewDocumentButton

A button that creates and opens new documents.

