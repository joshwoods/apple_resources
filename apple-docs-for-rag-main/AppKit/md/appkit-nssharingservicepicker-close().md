

- AppKit
- NSSharingServicePicker
-  close() 

Instance Method

# close()

Closes the picker interface.

macOS 13.0+

``` source
func close()
```

## Discussion

The sharingServicePicker(_:didChoose:) method will be invoked if the delegate is set to `nil`.

## See Also

### Displaying the sharing service picker

func show(relativeTo: NSRect, of: NSView, preferredEdge: NSRectEdge)

Shows the picker interface and populates it with the relevant sharing services.

