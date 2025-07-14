

- CarPlay
- CPInterfaceController
-  dismissTemplate(animated:completion:) 

Instance Method

# dismissTemplate(animated:completion:)

Dismisses a modal template.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func dismissTemplate(
    animated: Bool,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func dismissTemplate(animated: Bool) async throws -> Bool
```

## Parameters 

`animated`  

If true, CarPlay animates the dismissal of the template.

`completion`  

The closure CarPlay calls after it dismisses the template.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func dismissTemplate(animated: Bool) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

CarPlay calls `completion` after it dismisses the template. The Boolean parameter is true when the dismissal succeeds; otherwise, it’s false and CarPlay provides an error that describes the failure. CarPlay throws an exception if the dismissal fails and you don’t provide a closure.

## See Also

### Displaying Templates Modally

func presentTemplate(CPTemplate, animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Presents a template modally.

var presentedTemplate: CPTemplate?

The interface controller’s current modal template.

