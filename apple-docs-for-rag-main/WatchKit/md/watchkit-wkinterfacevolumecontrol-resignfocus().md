

- WatchKit
- WKInterfaceVolumeControl
-  resignFocus() 

Instance Method

# resignFocus()

Removes focus from the volume control, causing it to stop receiving input from the Digital Crown.

watchOS 6.0+

``` source
func resignFocus()
```

## Discussion

If the volume control is inside a scrollable view, resigning the focus enables scrolling with the Digital Crown.

## See Also

### Managing Input from the Digital Crown

func focus()

Sets the volume control as the focus for input from the Digital Crown.

