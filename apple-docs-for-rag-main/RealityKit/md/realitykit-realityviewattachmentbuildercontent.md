

- RealityKit
-  RealityViewAttachmentBuilderContent 

Structure

# RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
struct RealityViewAttachmentBuilderContent where Attachment : AttachmentContent, Content : View
```

## Overview

A RealityView creates this for you.

## Topics

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### SwiftUI view attachments

struct Attachment

An attachment content you can use to gather an identifier and view.

struct RealityViewAttachments

The attachments that belong to a RealityView.

class ViewAttachmentEntity

An entity that has a view attachment.

struct ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

struct TextComponent

A component that draws 2D text at an entity’s location.

