

- CarPlay
- CPInterfaceController
-  pushTemplate(\_:animated:completion:) 

Instance Method

# pushTemplate(\_:animated:completion:)

Adds the specified template to the navigation hierarchy and displays it.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func pushTemplate(
    _ templateToPush: CPTemplate,
    animated: Bool,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func pushTemplate(
    _ templateToPush: CPTemplate,
    animated: Bool
) async throws -> Bool
```

## Parameters 

`templateToPush`  

The template to add to the navigation hierarchy.

`animated`  

If true, CarPlay animates the transition between templates.

`completion`  

The closure CarPlay calls after it adds the template.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func pushTemplate(_ templateToPush: CPTemplate, animated: Bool) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

The template you add becomes the topTemplate in the navigation hierarchy.

CarPlay calls `completion` after it adds the template to the navigation hierarchy. The Boolean parameter is true when CarPlay adds the template successfully; otherwise, it’s false and CarPlay provides an error that describes the failure.

CarPlay throws an exception if it can’t add the template and you don’t provide a closure.

## See Also

### Adding and Removing Templates

func popTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes the top-most template from the navigation hierarchy.

func popToRootTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes all of the templates from the navigation hierarchy except the root template.

func pop(to: CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes each template from the navigation hierarchy until the specified template becomes visible.

