

- UIKit
- UIButton
-  systemButton(with:target:action:) 

Type Method

# systemButton(with:target:action:)

Creates and returns a system type button with specified image, target, and action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class func systemButton(
    with image: UIImage,
    target: Any?,
    action: Selector?
) -> Self
```

## Parameters 

`image`  

The image for a system button.

`target`  

The object that receives the `action` message.

`action`  

The action to send to `target` when this item is selected.

## Discussion

This method is a convenience constructor for creating a `UIButtonTypeSystem` type button objects with a specific target and action.

