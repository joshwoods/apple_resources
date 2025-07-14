

- Objective-C Runtime
- NSObject
-  handle(\_:client:) 

Instance Method

# handle(\_:client:)

Handles key down and mouse events.

macOS

``` source
func handle(
    _ event: NSEvent!,
    client sender: Any!
) -> Bool
```

## Parameters 

`event`  

The event to handle.

`sender`  

The client object sending the event.

## Return Value

YES if the event is handled; otherwise NO.

