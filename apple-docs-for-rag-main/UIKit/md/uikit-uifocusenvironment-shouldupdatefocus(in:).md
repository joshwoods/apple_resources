

- UIKit
- UIFocusEnvironment
-  shouldUpdateFocus(in:) 

Instance Method

# shouldUpdateFocus(in:)

Returns a Boolean value indicating whether the focus engine should allow the focus update described by the specified context to occur.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func shouldUpdateFocus(in context: UIFocusUpdateContext) -> Bool
```

**Required**

## Parameters 

`context`  

An instance of UIFocusUpdateContext class, containing metadata for the focus related update.

## Return Value

true to allow the focus update; otherwise, false.

## Discussion

When a focus update is about to occur, the focus engine calls this method on all focus environments that contain either the previously focused view, the next focused view, or both, in ascending order. If any environment returns false, the update is cancelled. Override this method to prevent the focus from moving to or from certain areas of the screen.

