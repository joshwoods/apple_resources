

- RealityKit
- RealityView
-  init(make:update:placeholder:) 

Initializer

# init(make:update:placeholder:)

Creates a new reality view for visionOS with an optional update closure and placeholder view.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
init(
    make: @escaping @MainActor (inout RealityViewContent) async -> Void,
    update: (@MainActor (inout RealityViewContent) -> Void)? = nil,
    @ViewBuilder placeholder: () -> P
) where Content == RealityViewContent.Body, P : View
```

Available when `Content` conforms to `View`.

## Parameters 

`make`  

An asynchronous closure that configures the initial content of the new `RealityView`. This closure is asynchronous to keep your app’s UI responsive while you load content to populate this view.

`update`  

An optional closure that updates the `RealityView` instance’s content as the view’s state changes.

`placeholder`  

A temporary view that the RealityView displays until your closure for the `make` parameter completes. For example, you can display a loading indicator with a ProgressView instance as a placeholder.

## Discussion

For example, your app can asynchronously load an Entity from a `.reality` or `.usdz` file, and display a ProgressView while the system loads the file:

```
RealityView { content in
    if let newEntity = try? await Entity(named: "model_file_name") {
        content.add(newEntity)
    }
} placeholder: {
    ProgressView()
}
```

## See Also

### Creating a reality view for visionOS

init(make: (inout RealityViewContent) async -> Void, update: ((inout RealityViewContent) -> Void)?)

Creates a new reality view for visionOS with an optional update closure.

init&lt;A>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, attachments: () -> A)

Creates a reality view for visionOS, with attachments and an optional update closure.

init&lt;A, P>(make: (inout RealityViewContent, RealityViewAttachments) async -> Void, update: ((inout RealityViewContent, RealityViewAttachments) -> Void)?, placeholder: () -> P, attachments: () -> A)

Creates a reality view for visionOS, with attachments, an optional update closure, and placeholder view.

