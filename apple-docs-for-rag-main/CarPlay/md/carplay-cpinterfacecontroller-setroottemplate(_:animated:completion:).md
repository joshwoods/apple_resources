

- CarPlay
- CPInterfaceController
-  setRootTemplate(\_:animated:completion:) 

Instance Method

# setRootTemplate(\_:animated:completion:)

Sets the root template of the navigation hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func setRootTemplate(
    _ rootTemplate: CPTemplate,
    animated: Bool,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func setRootTemplate(
    _ rootTemplate: CPTemplate,
    animated: Bool
) async throws -> Bool
```

## Parameters 

`rootTemplate`  

The template to use as the root of a new navigation hierarchy.

`animated`  

If true, CarPlay animates the presentation of the template. CarPlay ignores this flag when there isn’t an existing navigation hierarchy to replace.

`completion`  

The closure CarPlay calls after it presents the template.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func setRootTemplate(_ rootTemplate: CPTemplate, animated: Bool) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

If you set a root template when a navigation hierarchy already exists, CarPlay replaces the entire hierarchy.

CarPlay calls `completion` after it presents the template. The Boolean parameter is true when the presentation succeeds; otherwise, it’s false and CarPlay provides an error that describes the failure. CarPlay throws an exception if the presentation fails and you don’t provide a closure.

## See Also

### Configuring the Interface Controller

var delegate: (any CPInterfaceControllerDelegate)?

An object that serves as the delegate to the interface controller.

protocol CPInterfaceControllerDelegate

The interface that an object implements to serve as a delegate to an interface controller.

var prefersDarkUserInterfaceStyle: Bool

A Boolean value that determines whether the system draws the user interface in Dark Mode.

