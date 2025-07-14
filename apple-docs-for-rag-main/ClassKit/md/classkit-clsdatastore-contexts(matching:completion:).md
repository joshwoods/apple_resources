

- ClassKit
- CLSDataStore
-  contexts(matching:completion:) 

Instance Method

# contexts(matching:completion:)

Fetches all the contexts matching a predicate.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func contexts(
    matching predicate: NSPredicate,
    completion: @escaping ([CLSContext], (any Error)?) -> Void
)
```

``` source
func contexts(matching predicate: NSPredicate) async throws -> [CLSContext]
```

## Parameters 

`predicate`  

A predicate that the method uses to search for contexts.

`completion`  

A closure that the method calls with the array of contexts that match the predicate and an optional error that indicates the reason for failure, if any.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func contexts(matching predicate: NSPredicate) async throws -> [CLSContext]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use the predicate keys defined in CLSPredicateKeyPath to create a predicate that you pass to this method to search for contexts matching certain criteria.

For example, to print the titles of all the children of the main app context:

```
let store = CLSDataStore.shared
let predicate = NSPredicate(format: "%K = %@", CLSPredicateKeyPath.parent as CVarArg,
                                               store.mainAppContext)
store.contexts(matching: predicate) { contexts, _ in
    for context in contexts {
        print(context.title)
    }
}
```

Important

ClassKit calls your completion handler on an arbitrary thread. If you need to do work on a particular thread from inside the handler, dispatch that work to the appropriate queue.

## See Also

### Finding contexts that match criteria

func contexts(matchingIdentifierPath: [String], completion: ([CLSContext], (any Error)?) -> Void)

Fetches all the contexts along a given identifier path.

struct CLSPredicateKeyPath

The set of possible key paths you use to search for contexts.

