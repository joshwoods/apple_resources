

- ClassKit
- CLSDataStore
-  contexts(matchingIdentifierPath:completion:) 

Instance Method

# contexts(matchingIdentifierPath:completion:)

Fetches all the contexts along a given identifier path.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
func contexts(
    matchingIdentifierPath identifierPath: [String],
    completion: @escaping ([CLSContext], (any Error)?) -> Void
)
```

``` source
func contexts(matchingIdentifierPath identifierPath: [String]) async throws -> [CLSContext]
```

## Parameters 

`completion`  

A closure that the method calls with the matching contexts and an optional error that indicates the reason for failure, if any.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func contexts(matchingIdentifierPath identifierPath: [String]) async throws -> [CLSContext]
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to get all of the named contexts along the identifier path. For example:

```
let store = CLSDataStore.shared
store.contexts(matchingIdentifierPath: ["game", "level-1"]) { contexts, _ in
    for context in contexts {
        print(context.identifier)
    }
}
// Prints "game" and then "level-1"
```

The identifier path is taken starting from mainAppContext, which lies at the root of your app’s context hiearchy. For each context that doesn’t exist along the path, the data store calls its delegate’s createContext(forIdentifier:parentContext:parentIdentifierPath:) method to create the context. If contexts are missing and the data store has no delegate, the returned list of contexts is incomplete.

Important

ClassKit calls your completion handler on an arbitrary thread. If you need to do work on a particular thread from inside the handler, dispatch that work to the appropriate queue.

## See Also

### Finding contexts that match criteria

func contexts(matching: NSPredicate, completion: ([CLSContext], (any Error)?) -> Void)

Fetches all the contexts matching a predicate.

struct CLSPredicateKeyPath

The set of possible key paths you use to search for contexts.

