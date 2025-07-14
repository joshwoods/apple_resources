

- Media Player
- MPMediaPickerController
-  delegate 

Instance Property

# delegate

The delegate for a media item picker.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+

``` source
@MainActor
weak var delegate: (any MPMediaPickerControllerDelegate)? { get set }
```

## Discussion

Typically, you set the delegate to be the same object that initializes and displays the media item picker.

## See Also

### Responding to media item picker selections

protocol MPMediaPickerControllerDelegate

The protocol you implement so that a media item picker can respond to a user making media item selections.

