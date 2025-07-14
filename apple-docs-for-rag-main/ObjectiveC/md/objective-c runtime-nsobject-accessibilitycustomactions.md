

- Objective-C Runtime
- NSObject
-  accessibilityCustomActions 

Instance Property

# accessibilityCustomActions

An array of custom actions to display along with the built-in actions.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityCustomActions: [UIAccessibilityCustomAction]? { get set }
```

## Discussion

The array contains one or more `UIAccessibilityCustomAction` objects defining the supported actions. Assistive technologies, such as VoiceOver, display your custom actions to the user at appropriate times.

