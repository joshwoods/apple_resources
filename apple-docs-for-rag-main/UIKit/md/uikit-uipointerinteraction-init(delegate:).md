

- UIKit
- UIPointerInteraction
-  init(delegate:) 

Initializer

# init(delegate:)

Initializes a pointer interaction object with a specified delegate object.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
init(delegate: (any UIPointerInteractionDelegate)?)
```

## Parameters 

`delegate`  

An object the framework calls to respond to pointer movements.

## Discussion

If you create a `UIPointerInteraction` without a delegate by passing `nil` to the initializer, UIKit automatically applies a pointer effect it deems appropriate to the view. Initializing with `nil` is the equivalent of creating a `UIPointerStyle` with UIPointerEffect.automatic(_:). Based on the view’s appearance, `.automatic` transforms into one of the concrete effects (`.highlight`, `.lift`, `.hover`).

