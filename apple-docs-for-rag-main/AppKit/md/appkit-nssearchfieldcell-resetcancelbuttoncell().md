

- AppKit
- NSSearchFieldCell
-  resetCancelButtonCell() 

Instance Method

# resetCancelButtonCell()

Resets the cancel button cell to its default attributes.

macOS

``` source
@MainActor
func resetCancelButtonCell()
```

## Discussion

This method resets the target, action, regular image, and pressed image for the cancel button cell. By default, when users click the cancel button, the `delete:` action message is sent up the responder chain to the first `NSText` object that can handle it. This method gives you a way to customize the cancel button for specific situations and then reset the button defaults without having to undo changes individually.

## See Also

### Managing buttons

var searchButtonCell: NSButtonCell?

The button cell used to display the search-button image.

func resetSearchButtonCell()

Resets the search button cell to its default attributes.

var cancelButtonCell: NSButtonCell?

The button cell used to display the cancel-button image.

