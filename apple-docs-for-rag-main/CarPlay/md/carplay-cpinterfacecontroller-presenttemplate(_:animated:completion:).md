

- CarPlay
- CPInterfaceController
-  presentTemplate(\_:animated:completion:) 

Instance Method

# presentTemplate(\_:animated:completion:)

Presents a template modally.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
func presentTemplate(
    _ templateToPresent: CPTemplate,
    animated: Bool,
    completion: ((Bool, (any Error)?) -> Void)? = nil
)
```

``` source
func presentTemplate(
    _ templateToPresent: CPTemplate,
    animated: Bool
) async throws -> Bool
```

## Parameters 

`templateToPresent`  

The template to present modally.

`animated`  

If true, CarPlay animates the presentation of the template.

`completion`  

The closure CarPlay calls after it presents the template.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func presentTemplate(_ templateToPresent: CPTemplate, animated: Bool) async throws -> Bool
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

CarPlay can only present one modal template at a time. `templateToPresent` must be one of CPActionSheetTemplate, CPAlertTemplate, or CPVoiceControlTemplate.

CarPlay calls `completion` after it presents the template. The Boolean parameter is true when the presentation succeeds; otherwise, it’s false and CarPlay provides an error that describes the failure. CarPlay throws an exception if the presentation fails and you don’t provide a closure.

## See Also

### Displaying Templates Modally

func dismissTemplate(animated: Bool, completion: ((Bool, (any Error)?) -> Void)?)

Dismisses a modal template.

var presentedTemplate: CPTemplate?

The interface controller’s current modal template.

