

- SpriteKit
- SKViewDelegate
-  view(\_:shouldRenderAtTime:) 

Instance Method

# view(\_:shouldRenderAtTime:)

Specifies whether the view should render at the given time.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
optional func view(
    _ view: SKView,
    shouldRenderAtTime time: TimeInterval
) -> Bool
```

## Parameters 

`view`  

The SKView.

`time`  

The target time.

## Return Value

Return `true` to initiate an update and render for the target time. Return `false` to skip the update and render for the target time.

