

- RealityKit
- Entity
-  accessibilityLabel Deprecated

Instance Property

# accessibilityLabel

A succinct label that identifies the purpose of the image.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedvisionOSDeprecated

``` source
@MainActor @preconcurrency
var accessibilityLabel: String? { get set }
```

## Mentioned in 

Improving the Accessibility of RealityKit Apps

## Discussion

The default value for this property is `false`.

For entities with isAccessibilityElement set to true, iOS uses this string to provide information to users of assistive technologies like VoiceOver. Set this property to a name or short description that accurately describes the entity. If you wish to provide additional information or a longer description of the entity, you can use accessibilityDescription.

## See Also

### Configuring accessibility features

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

var isAccessibilityElement: Bool

A Boolean value indicating whether the receiver is an accessibility element that an assistive application can access.

var accessibilityLabelKey: LocalizedStringResource?

A succinct label that identifies the entity, in a localized string key.

var accessibilityCustomActions: [LocalizedStringResource]

An array of custom actions supported by the entity, identified by their localized string key.

var accessibilityCustomContent: [AccessibilityComponent.CustomContent]

The Custom Content API is useful for delivering accessibility information from complex data sets to your users in measured portions. Using this API allows you to leverage assistive technologies to present only the accessible content your app’s users need, when they need it.

var accessibilityCustomRotors: [AccessibilityComponent.RotorType]

An array of supported rotors.

var accessibilityLabelKey: LocalizedStringResource?

A succinct label that identifies the entity, in a localized string key.

var accessibilitySystemActions: AccessibilityComponent.SupportedActions

The set of supported accessibility actions.

var accessibilityTraits: UIAccessibilityTraits

The combination of accessibility traits that best characterize the entity.

var accessibilityValue: LocalizedStringResource?

A localized string key that represents the current value of the entity.

var accessibilityDescription: String?

A longer description of the entity for use by assistive technologies.

Deprecated

var accessibilityDescription: String?

A longer description of the entity for use by assistive technologies.

Deprecated

