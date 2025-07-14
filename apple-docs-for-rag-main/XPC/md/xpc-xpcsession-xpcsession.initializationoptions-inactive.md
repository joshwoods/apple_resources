

- XPC
- XPCSession
- XPCSession.InitializationOptions
-  inactive 

Type Property

# inactive

Indicates that the session isn’t activated during its creation.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
static var inactive: XPCSession.InitializationOptions
```

## Discussion

Important

If you create a session with this option, you must manually activate it by calling activate().

## See Also

### Session creation options

static var privileged: XPCSession.InitializationOptions

Indicates that the Mach service is in the priviledged Mach bootstrap.

static var none: XPCSession.InitializationOptions

Indicates that the listener uses a default configuration during creation.

