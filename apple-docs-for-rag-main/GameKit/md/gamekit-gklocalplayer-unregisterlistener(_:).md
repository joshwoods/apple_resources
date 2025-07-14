

- GameKit
- GKLocalPlayer
-  unregisterListener(\_:) 

Instance Method

# unregisterListener(\_:)

Unregisters a listener object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func unregisterListener(_ listener: any GKLocalPlayerListener)
```

## Parameters 

`listener`  

The object that GameKit stops sending messages to when events occur.

## See Also

### Registering Listeners

func register(any GKLocalPlayerListener)

Registers a listener for a particular event.

func unregisterAllListeners()

Unregisters all listeners in your game.

