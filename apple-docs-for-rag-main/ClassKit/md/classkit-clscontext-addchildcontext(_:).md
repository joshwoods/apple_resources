

- ClassKit
- CLSContext
-  addChildContext(\_:) 

Instance Method

# addChildContext(\_:)

Adds the specifed context as a child of the context receiving the method call.

iOS 11.4+iPadOS 11.4+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func addChildContext(_ child: CLSContext)
```

## Parameters 

`child`  

The context to add as a child of the one receiving the method call.

## Discussion

Typically you use the CLSDataStoreDelegate protocol to build contexts, in which case you don’t need to call this method directly.

## See Also

### Managing context hierarchy

var identifierPath: [String]

The identifier path that locates the context within the data store’s context hierarchy.

var parent: CLSContext?

The direct ancestor of this context.

func removeFromParent()

Removes the context from its parent.

func descendant(matchingIdentifierPath: [String], completion: (CLSContext?, (any Error)?) -> Void)

Finds the context with the given identifier path relative to this context.

