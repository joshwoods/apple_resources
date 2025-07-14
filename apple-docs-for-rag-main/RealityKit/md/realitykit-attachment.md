

- RealityKit
-  Attachment 

Structure

# Attachment

An attachment content you can use to gather an identifier and view.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct Attachment where Content : View
```

## Topics

### Initializers

init(id: AnyHashable, () -> Content)

Creates an new attachment from an identifier and a closure.

### Instance Properties

var content: Content

The view associated with this attachment.

var id: AnyHashable

The identifier of this attachment.

### Type Aliases

typealias Body

## Relationships

### Conforms To

- AttachmentContent

  Conforms when `Content` conforms to `View`.

- Copyable
- Sendable

## See Also

### SwiftUI view attachments

struct RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

struct RealityViewAttachments

The attachments that belong to a RealityView.

class ViewAttachmentEntity

An entity that has a view attachment.

struct ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

struct TextComponent

A component that draws 2D text at an entity’s location.

