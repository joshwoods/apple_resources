

- ClassKit
- CLSContext
-  descendant(matchingIdentifierPath:completion:) 

Instance Method

# descendant(matchingIdentifierPath:completion:)

Finds the context with the given identifier path relative to this context.

iOS 11.4+iPadOS 11.4+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func descendant(
    matchingIdentifierPath identifierPath: [String],
    completion: @escaping (CLSContext?, (any Error)?) -> Void
)
```

``` source
func descendant(matchingIdentifierPath identifierPath: [String]) async throws -> CLSContext
```

## Parameters 

`identifierPath`  

The identifier path of the context to find, relative to the current context.

`completion`  

A closure the method calls with the found context, or `nil` if none could be found, and an error indicating the reason for failure, if any.

## Mentioned in 

Recording student progress

Declaring your app’s context hierarchy

Building missing contexts

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func descendant(matchingIdentifierPath identifierPath: [String]) async throws -> CLSContext
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Important

ClassKit calls your completion handler on an arbitrary thread. If you need to do work on a particular thread from inside the handler, dispatch that work to the appropriate queue.

## See Also

### Managing context hierarchy

var identifierPath: [String]

The identifier path that locates the context within the data store’s context hierarchy.

var parent: CLSContext?

The direct ancestor of this context.

func removeFromParent()

Removes the context from its parent.

func addChildContext(CLSContext)

Adds the specifed context as a child of the context receiving the method call.

