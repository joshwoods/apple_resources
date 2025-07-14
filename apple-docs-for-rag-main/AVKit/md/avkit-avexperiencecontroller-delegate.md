

- AVKit
- AVExperienceController
-  delegate 

Instance Property

# delegate

A delegate object for the experience controller.

visionOS 2.0+

``` source
@MainActor
weak final var delegate: (any AVExperienceController.Delegate)? { get set }
```

## Discussion

Provide a delegate to have the system notify your app about transitions and other state changes. Use the delegate callbacks to update your app’s state and user interface in response.

## See Also

### Configuring a delegate

protocol Delegate

A protocol that defines the methods to implement to respond to experience changes.

