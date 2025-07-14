

- UIKit
- UIScribbleInteraction
-  isHandlingWriting 

Instance Property

# isHandlingWriting

A Boolean value that indicates whether the user is actively writing in a text view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
@MainActor
var isHandlingWriting: Bool { get }
```

## Discussion

This property is true in between calls to scribbleInteractionWillBeginWriting(_:) and scribbleInteractionDidFinishWriting(_:) when the user is writing.

