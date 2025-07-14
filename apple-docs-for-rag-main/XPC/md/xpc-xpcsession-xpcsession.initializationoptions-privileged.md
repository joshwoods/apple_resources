

- XPC
- XPCSession
- XPCSession.InitializationOptions
-  privileged 

Type Property

# privileged

Indicates that the Mach service is in the priviledged Mach bootstrap.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
static var privileged: XPCSession.InitializationOptions
```

## Discussion

The Mach service typically accomplishes this by placing its `launchd.plist` in the `LaunchDaemons` directory.

## See Also

### Session creation options

static var inactive: XPCSession.InitializationOptions

Indicates that the session isn’t activated during its creation.

static var none: XPCSession.InitializationOptions

Indicates that the listener uses a default configuration during creation.

