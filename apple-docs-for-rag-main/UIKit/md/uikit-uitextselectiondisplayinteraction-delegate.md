

- UIKit
- UITextSelectionDisplayInteraction
-  delegate 

Instance Property

# delegate

A delegate that provides a container view to manage the system-supplied selection views.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any UITextSelectionDisplayInteractionDelegate)? { get }
```

## Discussion

Provide a delegate object if your UI displays selection highlights below your text input view. The delegate provides the container view for the system to use when adding the selection-related views.

## See Also

### Managing the drawing view

protocol UITextSelectionDisplayInteractionDelegate

An object you use to customize the presentation of text selections in your interface.

