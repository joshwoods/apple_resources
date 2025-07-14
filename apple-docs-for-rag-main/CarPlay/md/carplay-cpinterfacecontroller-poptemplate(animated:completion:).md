

- CarPlay
- CPInterfaceController
-  popTemplate(animated:completion:) 

Instance Method

# popTemplate(animated:completion:)

Removes the top-most template from the navigation hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func popTemplate(
    animated: Bool,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func popTemplate(animated: Bool) async throws -> Bool
```

## Parameters 

`animated`  

If true, CarPlay animates the transition between templates.

`completion`  

The closure CarPlay calls after it removes the template.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func popTemplate(animated: Bool) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

CarPlay calls `completion` after it removes the top-most template from the navigation hierarchy. The Boolean parameter is true if CarPlay removes the template successfully; otherwise, it’s false and CarPlay provides an error that describes the failure.

CarPlay throws an exception if it can’t remove the template and you don’t provide a closure.

## See Also

### Adding and Removing Templates

func pushTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Adds the specified template to the navigation hierarchy and displays it.

func popToRootTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes all of the templates from the navigation hierarchy except the root template.

func pop(to: CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Removes each template from the navigation hierarchy until the specified template becomes visible.

