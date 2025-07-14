

- Core Haptics
- CHHapticEngine
-  stop(completionHandler:) 

Instance Method

# stop(completionHandler:)

Asynchronously stops the haptic engine and executes the completion handler once the engine has stopped.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func stop(completionHandler: CHHapticEngine.CompletionHandler? = nil)
```

``` source
func stop() async throws
```

## Parameters 

`completionHandler`  

The completion handler to execute after the engine stops.

## Mentioned in 

Preparing your app to play haptics

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func stop() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and Stopping the Haptic Engine

func start() throws

Synchronously starts the haptic engine.

func start(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously starts the haptic engine.

typealias CompletionHandler

A typealias for a completion handler that the engine calls after starting or stopping.

