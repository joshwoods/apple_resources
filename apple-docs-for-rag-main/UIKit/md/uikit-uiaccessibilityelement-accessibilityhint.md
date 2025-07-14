

- UIKit
- UIAccessibilityElement
-  accessibilityHint 

Instance Property

# accessibilityHint

A string that briefly describes the result of performing an action on the accessibility element.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityHint: String? { get set }
```

## Mentioned in 

Supporting VoiceOver in your app

## Discussion

The hint is a brief, localized description of the result of performing an action on the element without identifying the element or the action. For example, the hint for a table row that contains an email message might be “Selects the message,” but not “Tap this row to select the message.”

By default, standard UIKit controls and views have system-provided hints. If you provide a custom control or view, however, you need to set this property appropriately so that assistive applications can supply accurate information to users with disabilities.

## See Also

### Accessing the attributes of an accessibility element

var accessibilityLabel: String?

A string that succinctly identifies the accessibility element.

var accessibilityValue: String?

A string that represents the current value of the accessibility element.

var accessibilityFrame: CGRect

The frame of the accessibility element, in screen coordinates.

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

