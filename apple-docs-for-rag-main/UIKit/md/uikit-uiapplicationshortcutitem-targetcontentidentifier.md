

- UIKit
- UIApplicationShortcutItem
-  targetContentIdentifier 

Instance Property

# targetContentIdentifier

The object that determines which scene handles the quick action.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var targetContentIdentifier: Any? { get }
```

## Discussion

UIKit applies the value in this property to the activation conditions defined by the UISceneActivationConditions objects of the available scenes. Based on the predicates you specify, UIKit selects the most appropriate scene for handling the action.

