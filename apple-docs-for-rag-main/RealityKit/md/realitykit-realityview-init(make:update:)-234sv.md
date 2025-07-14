

- RealityKit
- RealityView
-  init(make:update:) 

Initializer

# init(make:update:)

Creates a reality view for iOS and macOS, with an optional update closure.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
nonisolated
init(
    make: @escaping @MainActor (inout RealityViewCameraContent) async -> Void,
    update: (@MainActor (inout RealityViewCameraContent) -> Void)? = nil
) where Content == RealityViewCameraContent.Body
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

### Creating a reality view for iOS and macOS

init&lt;P>(make: (inout RealityViewCameraContent) async -> Void, update: ((inout RealityViewCameraContent) -> Void)?, placeholder: () -> P)

Creates a reality view for iOS and macOS, with an optional update closure and placeholder view.

