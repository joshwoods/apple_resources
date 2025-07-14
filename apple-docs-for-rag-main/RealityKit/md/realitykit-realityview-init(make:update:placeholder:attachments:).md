

- RealityKit
- RealityView
-  init(make:update:placeholder:attachments:) 

Initializer

# init(make:update:placeholder:attachments:)

Creates a reality view for visionOS, with attachments, an optional update closure, and placeholder view.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    make: @escaping @MainActor (inout RealityViewContent, RealityViewAttachments) async -> Void,
    update: (@MainActor (inout RealityViewContent, RealityViewAttachments) -> Void)? = nil,
    @ViewBuilder placeholder: () -> P,
    @AttachmentContentBuilder attachments: @escaping () -> A
) where Content == RealityViewAttachmentBuilderContent>, A : AttachmentContent, P : View
```

Available when `Content` conforms to `View`.

## Parameters 

`make`  

An asynchronous closure that configures the initial content of the new `RealityView`. This closure is asynchronous to keep your app’s UI responsive while you load content to populate this view.

`update`  

An optional closure that updates the `RealityView` instance’s content as the view’s state changes.

`placeholder`  

A temporary view that the RealityView displays until your closure for the `make` parameter completes. For example, you can display a loading indicator with a ProgressView instance as a placeholder.

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

init&lt;A>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, attachments: () -> A)

Creates a reality view for visionOS, with attachments and an optional update closure.

