

- SwiftUI
- EditMode
-  EditMode.transient 

Case

# EditMode.transient

The view is in a temporary edit mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+tvOS 13.0+visionOS 1.0+

``` source
case transient
```

## Discussion

The use of this state varies by platform and for different controls. As an example, SwiftUI might engage temporary edit mode over the duration of a swipe gesture.

The isEditing property is `true` in this state.

## See Also

### Getting edit modes

case active

The user can edit the view content.

case inactive

The user can’t edit the view content.

