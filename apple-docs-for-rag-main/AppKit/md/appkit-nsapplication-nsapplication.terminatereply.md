

- AppKit
- NSApplication
-  NSApplication.TerminateReply 

Enumeration

# NSApplication.TerminateReply

Constants that determine whether an app should terminate.

macOS

``` source
enum TerminateReply
```

## Topics

### Constants

case terminateNow

It is OK to proceed with termination.

case terminateCancel

The app should not be terminated.

case terminateLater

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Terminating Applications

func applicationShouldTerminate(NSApplication) -> NSApplication.TerminateReply

Returns a value that indicates if the app should terminate.

func applicationShouldTerminateAfterLastWindowClosed(NSApplication) -> Bool

Returns a Boolean value that indicates if the app terminates once the last window closes.

func applicationWillTerminate(Notification)

Tells the delegate that the app is about to terminate.

