

- RealityKit
-  ViewAttachmentComponent 

Structure

# ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

RealityKitSwiftUIvisionOS 1.0+

``` source
struct ViewAttachmentComponent
```

## Topics

### Instance Properties

var bounds: BoundingBox

The bounding box of the view attachment, expressed in meters.

var id: AnyHashable

The identifier used for this view attachment.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component
- Identifiable
- TransientComponent

## See Also

### SwiftUI view attachments

struct RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

struct Attachment

An attachment content you can use to gather an identifier and view.

struct RealityViewAttachments

The attachments that belong to a RealityView.

class ViewAttachmentEntity

An entity that has a view attachment.

struct TextComponent

A component that draws 2D text at an entity’s location.

