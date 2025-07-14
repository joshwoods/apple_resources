

- ClassKit
- CLSContext
-  identifierPath 

Instance Property

# identifierPath

The identifier path that locates the context within the data store’s context hierarchy.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+

``` source
var identifierPath: [String] { get }
```

## Discussion

You can use the value stored in this property when calling the contexts(matchingIdentifierPath:completion:) method to retrieve the current context.

## See Also

### Managing context hierarchy

var parent: CLSContext?

The direct ancestor of this context.

func removeFromParent()

Removes the context from its parent.

func addChildContext(CLSContext)

Adds the specifed context as a child of the context receiving the method call.

func descendant(matchingIdentifierPath: [String], completion: (CLSContext?, (any Error)?) -> Void)

Finds the context with the given identifier path relative to this context.

