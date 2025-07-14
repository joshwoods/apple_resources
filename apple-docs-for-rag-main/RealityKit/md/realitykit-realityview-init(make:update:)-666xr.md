

- RealityKit
- RealityView
-  init(make:update:) 

Initializer

# init(make:update:)

Creates a new reality view for visionOS with an optional update closure.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    make: @escaping @MainActor (inout RealityViewContent) async -> Void,
    update: (@MainActor (inout RealityViewContent) -> Void)? = nil
) where Content == RealityViewContent.Body
```

Available when `Content` conforms to `View`.

## Parameters 

`make`  

An asynchronous closure that configures the initial content of the new `RealityView`. This closure is asynchronous to keep your app’s UI responsive while you load content to populate this view.

`update`  

An optional closure that updates the `RealityView` instance’s content as the view’s state changes.

## Discussion

Use the `update` closure to modify entities in the scene based on a Boolean state property, like in the following example:

```
RealityView { content in
    content.add(boxEntity)
} update: { content in
    boxEntity.scale = isEnlarged ? .one * 2 : .one
}
```

## See Also

### Creating a reality view for visionOS

init&lt;P>(make: (inout RealityViewContent) async -> Void, update: ((inout RealityViewContent) -> Void)?, placeholder: () -> P)

Creates a new reality view for visionOS with an optional update closure and placeholder view.

init&lt;A>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, attachments: () -> A)

Creates a reality view for visionOS, with attachments and an optional update closure.

init&lt;A, P>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, placeholder: () -> P, attachments: () -> A)

Creates a reality view for visionOS, with attachments, an optional update closure, and placeholder view.

