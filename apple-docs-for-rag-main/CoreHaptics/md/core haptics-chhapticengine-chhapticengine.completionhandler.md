

- Core Haptics
- CHHapticEngine
-  CHHapticEngine.CompletionHandler 

Type Alias

# CHHapticEngine.CompletionHandler

A typealias for a completion handler that the engine calls after starting or stopping.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOStvOS 14.0+visionOS 1.0+

``` source
typealias CompletionHandler = ((any Error)?) -> Void
```

## See Also

### Starting and Stopping the Haptic Engine

func start() throws

Synchronously starts the haptic engine.

func start(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously starts the haptic engine.

func stop(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously stops the haptic engine and executes the completion handler once the engine has stopped.

