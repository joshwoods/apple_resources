

- ClassKit
- CLSDataStore
-  save(completion:) 

Instance Method

# save(completion:)

Saves any changes you’ve made in the data store.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func save(completion: (((any Error)?) -> Void)? = nil)
```

``` source
func save() async throws
```

## Parameters 

`completion`  

A closure the method calls on completion of the save operation with an optional error value that indicates the reason for failure, if any.

## Mentioned in 

Recording student progress

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func save() async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

ClassKit calls your completion handler on an arbitrary thread. If you need to do work on a particular thread from inside the handler, dispatch that work to the appropriate queue.

