

- Core Haptics
- CHHapticEngine
-  start() 

Instance Method

# start()

Synchronously starts the haptic engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func start() throws
```

## Mentioned in 

Playing a single-tap haptic pattern

Preparing your app to play haptics

## Discussion

This method blocks all subsequent event processing on the current thread until the engine has started. It throws an error if the engine can’t start.

## See Also

### Starting and Stopping the Haptic Engine

func start(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously starts the haptic engine.

func stop(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously stops the haptic engine and executes the completion handler once the engine has stopped.

typealias CompletionHandler

A typealias for a completion handler that the engine calls after starting or stopping.

