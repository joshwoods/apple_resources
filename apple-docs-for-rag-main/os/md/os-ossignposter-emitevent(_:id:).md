

- os
- OSSignposter
-  emitEvent(\_:id:) 

Instance Method

# emitEvent(\_:id:)

Marks a point of interest in time.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func emitEvent(
    _ name: StaticString,
    id: OSSignpostID = .exclusive
)
```

## Parameters 

`name`  

The event’s name.

`id`  

The event’s identifier. The default value is exclusive.

## Mentioned in 

Recording Performance Data

## Discussion

You can use the makeSignpostID() and makeSignpostID(from:) methods to generate an identifier for the event, as the following example shows:

```
// Create a signposter using the default subsystem.
let signposter = OSSignposter()

// Generate a signpost ID to associate with the event.
let signpostID = signposter.makeSignpostID()

// Emit a named event using the signpost ID.
signposter.emitEvent("Example Event", id: signpostID)
```

## See Also

### Emitting Individual Signposts

func emitEvent(StaticString, id: OSSignpostID, SignpostMetadata)

Marks a point of interest in time and attaches the specified message.

