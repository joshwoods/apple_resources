

- Contacts UI
- CNContactPicker
-  showRelative(to:of:preferredEdge:) 

Instance Method

# showRelative(to:of:preferredEdge:)

Shows the picker popover anchored to the specified view.

macOS 10.11+

``` source
func showRelative(
    to positioningRect: NSRect,
    of positioningView: NSView,
    preferredEdge: NSRectEdge
)
```

## Parameters 

`positioningRect`  

The content size of the popover.

`positioningView`  

The view to which the popover should be positioned.

`preferredEdge`  

The edge to which the popover should be anchored to.

## See Also

### Related Documentation

@MainActor class NSPopover

A means to display additional content related to existing content on the screen.

