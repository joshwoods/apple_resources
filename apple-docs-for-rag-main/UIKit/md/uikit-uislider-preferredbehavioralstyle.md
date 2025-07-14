

- UIKit
- UISlider
-  preferredBehavioralStyle 

Instance Property

# preferredBehavioralStyle

The preferred behavioral style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var preferredBehavioralStyle: UIBehavioralStyle { get set }
```

## Mentioned in 

Choosing a user interface idiom for your Mac app

## Discussion

Use this property to specify the behavioral style for the slider. If the value of the property is UIBehavioralStyle.automatic, use the behavioralStyle property to determine the actual style.

The default value for preferredBehavioralStyle is UIBehavioralStyle.automatic. To learn more about behavior styles, see UIBehavioralStyle.

## See Also

### Modifying the slider’s behavior

var isContinuous: Bool

A Boolean value indicating whether changes in the slider’s value generate continuous update events.

var behavioralStyle: UIBehavioralStyle

The style that determines how the slider behaves.

enum UIBehavioralStyle

Constants that indicate how a control behaves in apps built with Mac Catalyst.

