

- UIKit
- UIPresentationController
-  adaptivePresentationStyle(for:) 

Instance Method

# adaptivePresentationStyle(for:)

Returns the presentation style to use for the specified set of traits.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func adaptivePresentationStyle(for traitCollection: UITraitCollection) -> UIModalPresentationStyle
```

## Parameters 

`traitCollection`  

The traits for the target environment.

## Return Value

The value provided by the presentation controller’s delegate or UIModalPresentationStyle.none if a delegate was not provided or does not return a valid value.

## Discussion

After the content managed by the presentation controller is onscreen, this method returns the presentation style to use for the specified set of traits. The default implementation of this method consults its delegate object and returns the value returned by that object’s `adaptivePresentationStyleForPresentationController:traitCollection:` method. Some system-supplied presentation controllers may also provide a new style that is more suited to the new set of traits.

This method returns the presentation style for the new traits, but does not initiate a transition to the new style. The system initiates the transition to the new style when the traits actually change. When transitioning to new traits, the actual presentation controller object may change. As a result, do not cache the presentation controller object in your code. Always retrieve it from your view controller’s presentationController property.

## See Also

### Getting the presentation attributes

var presentationStyle: UIModalPresentationStyle

The presentation style of the presented view controller.

var adaptivePresentationStyle: UIModalPresentationStyle

Returns the presentation style to use when the presented view controller becomes horizontally compact.

var shouldPresentInFullscreen: Bool

A Boolean value indicating whether the presentation covers the entire screen.

var shouldRemovePresentersView: Bool

A Boolean value indicating whether the presenting view controller’s view should be removed when the presentation animations finish.

