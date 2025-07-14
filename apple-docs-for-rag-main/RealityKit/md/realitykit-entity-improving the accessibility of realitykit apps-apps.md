

- RealityKit
- Entity
-  Improving the Accessibility of RealityKit Apps 

Article

# Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

## Overview

To support assistive technologies such as VoiceOver in your RealityKit apps, set the properties on each visible Entity in your scene. You can configure accessibility in Reality Composer, and in code.

Note

To see an example of accessibility support in a RealityKit app, check out the \Configuring Collision in RealityKit\> sample code project.

### Configure accessibility in Reality Composer

When you create a scene in Reality Composer, you can configure the accessibility properties of your entities right in the properties inspector. Select one or more entities in your scene and click the Accessibility Enabled checkbox in the properties inspector. In the Label field, give the entity a name to be used by assistive technologies. In the Detailed Description field, you can optionally add a more in-depth description.

### Configure accessibility in code

You can also configure entities to work with assistive technologies in code. To enable accessibility support for an Entity, set its isAccessibilityElement property to `True` and provide a short descriptive name using accessibilityLabel. If you want to provide a more detailed description, set accessibilityDescription.

Because these properties were introduced in iOS 14, any code that sets or reads their values should be wrapped in an availability macro if your project’s deployment target is iOS 13. Setting these values on an older version of iOS results in a runtime exception.

```
if #available(iOS 14.0, *) {
    ball.isAccessibilityElement = true
    ball.accessibilityLabel = "a bowling ball"
    ball.accessibilityDescription = "Tap and drag to roll the ball towards the pins."
}
```

## See Also

### Related Documentation

Configuring Collision in RealityKit

Use collision groups and collision filters to control which objects collide.

### Configuring accessibility features

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

var accessibilityLabel: String?

A succinct label that identifies the purpose of the image.

Deprecated

var accessibilityDescription: String?

A longer description of the entity for use by assistive technologies.

Deprecated

