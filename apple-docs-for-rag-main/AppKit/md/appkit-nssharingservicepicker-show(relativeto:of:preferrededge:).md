

- AppKit
- NSSharingServicePicker
-  show(relativeTo:of:preferredEdge:) 

Instance Method

# show(relativeTo:of:preferredEdge:)

Shows the picker interface and populates it with the relevant sharing services.

macOS 10.8+

``` source
func show(
    relativeTo rect: NSRect,
    of view: NSView,
    preferredEdge: NSRectEdge
)
```

## Parameters 

`rect`  

The rectangle the picker should be showed relative to. The coordinates are in the `view` coordinate system. Passing NSZeroRect causes the view bounds to be used.

`view`  

The view.

`preferredEdge`  

The preferred edge of the view to display the picker. See NSRectEdge for the possible values.

## Discussion

In macOS 13 and later, the picker displays the macOS share sheet in a popover. In earlier versions of macOS, the picker displays a menu with the available services. When someone chooses a service for sharing the items, the picker notifies its delegate and then shares the content.

The following example shows the basic code to display the picker in response to an action. Update the code to include the items you want to share and to position the picker interface in an appropriate part of your window.

```
- (IBAction)share:(id)sender
{
    NSArray * items = @[];
    NSSharingServicePicker * picker = [[NSSharingServicePicker alloc] initWithItems:items];
    picker.delegate = self;
    [picker showRelativeToRect:[sender bounds] ofView:sender preferredEdge:NSMinYEdge];
}
```

## See Also

### Displaying the sharing service picker

func close()

Closes the picker interface.

