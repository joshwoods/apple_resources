

- ClassKit
- CLSContext
-  removeFromParent() 

Instance Method

# removeFromParent()

Removes the context from its parent.

iOS 11.4+iPadOS 11.4+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func removeFromParent()
```

## Discussion

If you remove a context from its parent and don’t add it as the child of another context before you call save(completion:), then the framework deletes the context entirely.

## See Also

### Managing context hierarchy

var identifierPath: [String]

The identifier path that locates the context within the data store’s context hierarchy.

var parent: CLSContext?

The direct ancestor of this context.

func addChildContext(CLSContext)

Adds the specifed context as a child of the context receiving the method call.

func descendant(matchingIdentifierPath: [String], completion: (CLSContext?, (any Error)?) -> Void)

Finds the context with the given identifier path relative to this context.

