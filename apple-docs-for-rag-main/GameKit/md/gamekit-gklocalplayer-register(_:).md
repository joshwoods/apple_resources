

- GameKit
- GKLocalPlayer
-  register(\_:) 

Instance Method

# register(\_:)

Registers a listener for a particular event.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
func register(_ listener: any GKLocalPlayerListener)
```

## Parameters 

`listener`  

The object that GameKit sends messages to when events occur.

## Discussion

Only register a listener a single time. Registering a listener multiple times results in undefined behavior.

## See Also

### Registering Listeners

func unregisterAllListeners()

Unregisters all listeners in your game.

func unregisterListener(any GKLocalPlayerListener)

Unregisters a listener object.

