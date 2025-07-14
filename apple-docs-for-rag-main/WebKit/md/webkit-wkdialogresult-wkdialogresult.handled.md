

- WebKit
- WKDialogResult
-  WKDialogResult.handled 

Case

# WKDialogResult.handled

A result that indicates the delegate displayed the first use message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
case handled
```

## Discussion

This result tells the system that it does not need to check any more whether it needs to display the Lockdown Mode first use message.

## See Also

### First use dialog results

case askAgain

A result that indicates the delegate didn’t display a message, so other web views should check again.

case showDefault

A result that indicates the delegate didn’t display a message, so the web view should show the default Lockdown Mode message.

