

- AppKit
- NSApplication
- NSApplication.TerminateReply
-  NSApplication.TerminateReply.terminateLater 

Case

# NSApplication.TerminateReply.terminateLater

macOS

``` source
case terminateLater
```

## Discussion

It may be OK to proceed with termination later. Returning this value causes Cocoa to run the run loop in the NSModalPanelRunLoopMode until your app subsequently calls reply(toApplicationShouldTerminate:) with the value true or false. This return value is for delegates that need to provide document modal alerts (sheets) in order to decide whether to quit.

## See Also

### Constants

case terminateNow

It is OK to proceed with termination.

case terminateCancel

The app should not be terminated.

