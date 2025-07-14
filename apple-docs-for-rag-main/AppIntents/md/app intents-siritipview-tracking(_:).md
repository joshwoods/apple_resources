

- App Intents
- SiriTipView
-  tracking(\_:) 

Instance Method

# tracking(\_:)

Sets the tracking for the text in this view.

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func tracking(_ tracking: CGFloat) -> some View
```

## Parameters 

`tracking`  

The amount of additional space, in points, that the view should add to each character cluster after layout. Value of `0` sets the tracking to the system default value.

## Return Value

A view where text has the specified amount of tracking.

