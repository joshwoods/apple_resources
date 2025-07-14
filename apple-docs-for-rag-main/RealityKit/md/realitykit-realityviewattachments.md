

- RealityKit
-  RealityViewAttachments 

Structure

# RealityViewAttachments

The attachments that belong to a RealityView.

RealityKitSwiftUIvisionOS 1.0+

``` source
struct RealityViewAttachments
```

## Overview

Use this type to access entities associated with the attachments you provide to your RealityView via the init(make:update:attachments:) initializer.

## Topics

### Instance Methods

func entity(for: some Hashable) -> ViewAttachmentEntity?

Gets the identified attachment view as an entity, if the view with that identifier exists.

## See Also

### SwiftUI view attachments

struct RealityViewAttachmentBuilderContent

A view that gathers the attachment content for your current reality view.

struct Attachment

An attachment content you can use to gather an identifier and view.

class ViewAttachmentEntity

An entity that has a view attachment.

struct ViewAttachmentComponent

A component containing additional information about a view attachment entity provided via the entity(for:) function.

struct TextComponent

A component that draws 2D text at an entity’s location.

