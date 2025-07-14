

- AppKit
- NSPopover
- NSPopover.Behavior
-  NSPopover.Behavior.transient 

Case

# NSPopover.Behavior.transient

The system will close the popover when the user interacts with a user interface element outside the popover.

macOS

``` source
case transient
```

## Discussion

Note that interacting with menus or panels that become key only when needed will not cause a transient popover to close. The exact interactions that will cause transient popovers to close are not specified.

## See Also

### Constants

case applicationDefined

Your application assumes responsibility for closing the popover.

case semitransient

The system will close the popover when the user interacts with user interface elements in the window containing the popover’s positioning view.

