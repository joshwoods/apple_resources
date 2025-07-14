

- os
- OSSignposter
-  emitEvent(\_:id:\_:) 

Instance Method

# emitEvent(\_:id:\_:)

Marks a point of interest in time and attaches the specified message.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func emitEvent(
    _ name: StaticString,
    id: OSSignpostID = .exclusive,
    _ message: SignpostMetadata
)
```

## Parameters 

`name`  

The event’s name.

`id`  

The event’s identifier. The default value is exclusive.

`message`  

The interpolated string that the signposter attaches to the event. Each of the message’s interpolations can specify individual formatting and privacy options. For more information, see Message Argument Formatters.

## Discussion

Important

Don’t create an instance of SignpostMetadata. Instead, provide an interpolated string as the `message` parameter and the system converts it automatically.

You can use the makeSignpostID() and makeSignpostID(from:) methods to generate an identifier for the event, as the following example shows:

```
let accountNumber = "12345678"

// Create a signposter using the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the event.
let signpostID = signposter.makeSignpostID()

// Emit a named event using the signpost ID and attach a message
// that securely interpolates sensitive data.
signposter.emitEvent("New Account Created", id: signpostID,
    "Account: \(accountNumber, privacy: .sensitive(mask: .hash))")
```

## See Also

### Emitting Individual Signposts

func emitEvent(StaticString, id: OSSignpostID)

Marks a point of interest in time.

