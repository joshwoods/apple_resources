

- UIKit
- UISlider
-  isContinuous 

Instance Property

# isContinuous

A Boolean value indicating whether changes in the slider’s value generate continuous update events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isContinuous: Bool { get set }
```

## Discussion

If true, the slider triggers the associated target’s action method repeatedly, as the user moves the thumb. If false, the slider triggers the associated action method just once, when the user releases the slider’s thumb control to set the final value.

The default value of this property is true.

## See Also

### Modifying the slider’s behavior

var behavioralStyle: UIBehavioralStyle

The style that determines how the slider behaves.

var preferredBehavioralStyle: UIBehavioralStyle

The preferred behavioral style.

enum UIBehavioralStyle

Constants that indicate how a control behaves in apps built with Mac Catalyst.

