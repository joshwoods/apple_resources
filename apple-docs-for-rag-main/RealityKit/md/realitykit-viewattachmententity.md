

- RealityKit
-  ViewAttachmentEntity 

Class

# ViewAttachmentEntity

An entity that has a view attachment.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
class ViewAttachmentEntity
```

## Topics

### Instance Properties

var attachment: ViewAttachmentComponent

The view attachment component for this entity.

## Relationships

### Inherits From

- Entity

### Conforms To

- CustomDebugStringConvertible
- Equatable
- EventSource
- HasHierarchy
- HasSynchronization
- HasTransform
- Hashable
- Identifiable
- RealityCoordinateSpace
- Sendable

## See Also

### SwiftUI view attachments

struct RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

struct Attachment

An attachment content you can use to gather an identifier and view.

struct RealityViewAttachments

The attachments that belong to a RealityView.

struct ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

struct TextComponent

A component that draws 2D text at an entity’s location.

