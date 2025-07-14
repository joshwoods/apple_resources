

- Game Controller
- GCVirtualController
-  connect(replyHandler:) 

Instance Method

# connect(replyHandler:)

Connects the virtual controller to the device and displays it on the screen.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func connect(replyHandler reply: (((any Error)?) -> Void)? = nil)
```

``` source
func connect() async throws
```

## Parameters 

`reply`  

A closure that the method calls upon completion with the following parameter:

`error`  
Describes an error if it occurs, or returns `nil` if the operation completes.

## Mentioned in 

Adding touch controls to games that support game controllers in iOS

## Discussion

After you invoke this method, the framework calls any input handlers you set for the elements, or you can poll the elements for their values.

## See Also

### Connecting and displaying virtual controllers

func disconnect()

Disconnects the virtual controller from the device and removes it from the screen.

