

- AppKit
- NSPopover
- NSPopover.Behavior
-  NSPopover.Behavior.applicationDefined 

Case

# NSPopover.Behavior.applicationDefined

Your application assumes responsibility for closing the popover.

macOS

``` source
case applicationDefined
```

## Discussion

The system will still close the popover in a limited number of circumstances. For instance, the system will attempt to close the popover when the window of its positioningView is closed. The exact interactions in which AppKit will close the popover are not guaranteed. You may consider implementing -cancel: to close the popover when the escape key is pressed.

## See Also

### Constants

case transient

The system will close the popover when the user interacts with a user interface element outside the popover.

case semitransient

The system will close the popover when the user interacts with user interface elements in the window containing the popover’s positioning view.

