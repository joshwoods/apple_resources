

- AppKit
- NSTableViewRowAction
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the action button.

macOS 10.11+

``` source
@NSCopying
var backgroundColor: NSColor! { get set }
```

## Discussion

Use this property to specify the background color for your button. If you do not specify a value for this property, AppKit assigns a default color based on the value in the style property. Generally, this color is red for destructive actions and blue for nondestructive actions.

## See Also

### Configuring the Action’s Appearance

var style: NSTableViewRowAction.Style

The style applied to the action button.

var title: String

The title of the action button.

