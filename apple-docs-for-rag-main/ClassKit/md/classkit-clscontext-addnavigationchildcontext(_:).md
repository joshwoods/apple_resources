

- ClassKit
- CLSContext
-  addNavigationChildContext(\_:) 

Instance Method

# addNavigationChildContext(\_:)

Adds a child context that users can navigate to from this context.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
func addNavigationChildContext(_ child: CLSContext)
```

## Parameters 

`child`  

A context that you want to add as a presentable child from this context.

## Discussion

Use this method to add a child to the navigationChildContexts collection of a given context. This only affects presentation. The method doesn’t alter your app’s context hierarchy because it has no effect on the context’s identifierPath.

## See Also

### Creating a context presentation hierarchy

var navigationChildContexts: [CLSContext]

The child contexts that a user can navigate to from this context in the Schoolwork app.

func removeNavigationChildContext(CLSContext)

Removes the specified context as a presentable child of this context.

