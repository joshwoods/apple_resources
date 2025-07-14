

- AppKit
- NSTableView
-  register(\_:forIdentifier:) 

Instance Method

# register(\_:forIdentifier:)

Registers a NIB for the specified identifier, so that view-based table views can use it to instantiate views.

macOS 10.8+

``` source
@MainActor
func register(
    _ nib: NSNib?,
    forIdentifier identifier: NSUserInterfaceItemIdentifier
)
```

## Parameters 

`nib`  

The nib containing the view.

`identifier`  

The identifier of the view to create.

## Discussion

Use this method to associate one of the NIB’s cell views with `identifier` so that the table can instantiate this view when requested. This method is used when makeView(withIdentifier:owner:) is called, and there was no NIB created at design time for the specified identifier. This allows dynamic loading of NIBs that can be associated with the table.

Because a NIB can contain multiple views, you can associate the same NIB with multiple identifiers. To remove a previously associated NIB for `identifier`, pass in `nil` for the `nib` value.

Note

This method applies only to NSView-based table views.

## See Also

### NSView-Based Table Nib File Registration

var registeredNibsByIdentifier: [NSUserInterfaceItemIdentifier : NSNib]?

The dictionary of all registered nib files for view-based table view identifiers.

