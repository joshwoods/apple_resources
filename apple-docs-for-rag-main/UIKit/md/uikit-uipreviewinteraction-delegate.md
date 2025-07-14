

- UIKit
- UIPreviewInteraction
-  delegate 

Instance Property

# delegate

An object that acts as the delegate of the preview interaction.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UIPreviewInteractionDelegate)? { get set }
```

## Discussion

The preview interaction informs the delegate of state and progress changes throughout the 3D Touch process. Create an object that conforms to the UIPreviewInteractionDelegate protocol and assign it to this property.

## See Also

### Preparing preview interactions

protocol UIPreviewInteractionDelegate

A set of methods for communicating the progress of a preview interaction.

