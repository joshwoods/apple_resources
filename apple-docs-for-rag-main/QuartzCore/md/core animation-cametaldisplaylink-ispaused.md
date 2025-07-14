

- Core Animation
- CAMetalDisplayLink
-  isPaused 

Instance Property

# isPaused

A Boolean value that indicates whether the system suspends the display link’s notifications to the target.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var isPaused: Bool { get set }
```

## Discussion

You can instruct the display link to stop sending notifications to the delegate by setting the property to true. The property defaults to false.

