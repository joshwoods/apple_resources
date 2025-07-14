

- RealityKit
- RealityView
-  init(make:update:attachments:) 

Initializer

# init(make:update:attachments:)

Creates a reality view for visionOS, with attachments and an optional update closure.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    make: @escaping @MainActor (inout RealityViewContent, RealityViewAttachments) async -> Void,
    update: (@MainActor (inout RealityViewContent, RealityViewAttachments) -> Void)? = nil,
    @AttachmentContentBuilder attachments: @escaping () -> A
) where Content == RealityViewAttachmentBuilderContent>, A : AttachmentContent
```

Available when `Content` conforms to `View`.

## Parameters 

`make`  

An asynchronous closure that configures the initial content of the new `RealityView`. This closure is asynchronous to keep your app’s UI responsive while you load content to populate this view.

`update`  

An optional closure that updates the `RealityView` instance’s content as the view’s state changes.

`attachments`  

An attachment content builder that adds attachment views to the content of the `RealityView`.

## Discussion

This initializer doesn’t automatically add the attachment views to your RealityViewContent. You can access the entities that represent the attachments by calling the entity(for:) method of the RealityViewAttachments, and add them to your content or as a child of another Entity:

```
RealityView { content, attachments in
    if let attachment = attachments.entity(for: "example") {
        content.add(attachment)
    }
} attachments: {
    Attachment(id: "example") {
        Text("hello")
    }
}
```

## See Also

### Creating a reality view for visionOS

init(make: (inout RealityViewContent) async -> Void, update: ((inout RealityViewContent) -> Void)?)

Creates a new reality view for visionOS with an optional update closure.

init&lt;P>(make: (inout RealityViewContent) async -> Void, update: ((inout RealityViewContent) -> Void)?, placeholder: () -> P)

Creates a new reality view for visionOS with an optional update closure and placeholder view.

init&lt;A, P>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, placeholder: () -> P, attachments: () -> A)

Creates a reality view for visionOS, with attachments, an optional update closure, and placeholder view.

