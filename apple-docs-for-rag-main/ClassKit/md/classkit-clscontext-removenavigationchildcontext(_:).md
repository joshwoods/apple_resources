

- ClassKit
- CLSContext
-  removeNavigationChildContext(\_:) 

Instance Method

# removeNavigationChildContext(\_:)

Removes the specified context as a presentable child of this context.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
func removeNavigationChildContext(_ child: CLSContext)
```

## Parameters 

`child`  

The context that you want to remove as a presentable child of this context.

## Discussion

Use this method to remove a child from the navigationChildContexts collection of a given context. This only affects presentation. The method doesn’t alter your app’s context hierarchy because it has no effect on the context’s identifierPath.

## See Also

### Creating a context presentation hierarchy

var navigationChildContexts: [CLSContext]

The child contexts that a user can navigate to from this context in the Schoolwork app.

func addNavigationChildContext(CLSContext)

Adds a child context that users can navigate to from this context.

