

- Game Controller
- GCVirtualController
-  disconnect() 

Instance Method

# disconnect()

Disconnects the virtual controller from the device and removes it from the screen.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func disconnect()
```

## Discussion

After you invoke this method, the framework stops calling input handlers that you set for the elements.

## See Also

### Connecting and displaying virtual controllers

func connect(replyHandler: (((any Error)?) -> Void)?)

Connects the virtual controller to the device and displays it on the screen.

