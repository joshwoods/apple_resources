

- Core Image
- CIContext
- CIContextOption
-  priorityRequestLow 

Type Property

# priorityRequestLow

A key for enabling low-priority GPU use.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.12+tvOS 9.0+visionOS 1.0+

``` source
static let priorityRequestLow: CIContextOption
```

## Discussion

The value for this key is an NSNumber object containing a Boolean value. If this value is `true`, use of the Core Image context from a background thread takes lower priority than GPU usage from the main thread, allowing your app to perform Core Image rendering without disturbing the frame rate of UI animations.

