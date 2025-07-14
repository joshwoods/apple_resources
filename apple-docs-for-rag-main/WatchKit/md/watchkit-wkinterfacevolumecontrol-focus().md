

- WatchKit
- WKInterfaceVolumeControl
-  focus() 

Instance Method

# focus()

Sets the volume control as the focus for input from the Digital Crown.

watchOS 6.0+

``` source
func focus()
```

## Discussion

When the volume control has the focus, the system highlights it. The user can then use the Digital Crown to increase or decrease the volume.

## See Also

### Managing Input from the Digital Crown

func resignFocus()

Removes focus from the volume control, causing it to stop receiving input from the Digital Crown.

