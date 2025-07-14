

- Foundation
- NSXPCConnection
- NSXPCConnection.Options
-  privileged 

Type Property

# privileged

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var privileged: NSXPCConnection.Options { get }
```

## Discussion

Use this option if connecting to a service in the privileged Mach bootstrap (for example, a daemon with a `launchd.plist` in `/Library/LaunchDaemons)`.

