

- Core Haptics
- CHHapticEngine
-  start(completionHandler:) 

Instance Method

# start(completionHandler:)

Asynchronously starts the haptic engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func start(completionHandler: CHHapticEngine.CompletionHandler? = nil)
```

``` source
func start() async throws
```

## Parameters 

`completionHandler`  

The closure the system calls to indicate whether the server started successfully or encountered an error.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func start() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Starting and Stopping the Haptic Engine

func start() throws

Synchronously starts the haptic engine.

func stop(completionHandler: CHHapticEngine.CompletionHandler?)

Asynchronously stops the haptic engine and executes the completion handler once the engine has stopped.

typealias CompletionHandler

A typealias for a completion handler that the engine calls after starting or stopping.

