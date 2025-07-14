

- ClassKit
- CLSContext
-  parent 

Instance Property

# parent

The direct ancestor of this context.

iOS 11.4+iPadOS 11.4+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
weak var parent: CLSContext? { get }
```

## See Also

### Managing context hierarchy

var identifierPath: [String]

The identifier path that locates the context within the data store’s context hierarchy.

func removeFromParent()

Removes the context from its parent.

func addChildContext(CLSContext)

Adds the specifed context as a child of the context receiving the method call.

func descendant(matchingIdentifierPath: [String], completion: (CLSContext?, (any Error)?) -> Void)

Finds the context with the given identifier path relative to this context.

