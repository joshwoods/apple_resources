

- AppKit
- NSPopover
- NSPopover.Behavior
-  NSPopover.Behavior.semitransient 

Case

# NSPopover.Behavior.semitransient

The system will close the popover when the user interacts with user interface elements in the window containing the popover’s positioning view.

macOS

``` source
case semitransient
```

## Discussion

Semi-transient popovers cannot be shown relative to views in other popovers, nor can they be shown relative to views in child windows. The exact interactions that cause semi-transient popovers to close are not specified.

## See Also

### Constants

case applicationDefined

Your application assumes responsibility for closing the popover.

case transient

The system will close the popover when the user interacts with a user interface element outside the popover.

