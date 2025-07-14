

- UIKit
- Touches, presses, and gestures
- Coordinating multiple gesture recognizers
-  Attaching gesture recognizers to UIKit controls 

Article

# Attaching gesture recognizers to UIKit controls

Learn how gesture recognizers interact with UIKit controls such as buttons switches and sliders.

## Overview

Gesture recognizers attached to your views don’t impact the ability of UIKit controls to handle events. Events occurring within the bounds of a control are handled by the control first, giving the control a chance to call its action method. Specifically, UIKit controls call their action method in the following situations:

- A single finger single tap occurs on a UIButton, UISwitch, UIStepper, UISegmentedControl, or UIPageControl object.

- A single finger swipe occurs on the knob of a UISlider object, in a direction parallel to the slider.

- A single finger pan occurs on the knob of a UISwitch object, in a direction parallel to the switch.

To handle any of the preceding gestures before the control calls its action method, install your gesture recognizer on the control itself. Gesture recognizers handle touch events before the views to which they’re attached. As a result, installing a gesture recognizer directly on a control prevents that control from calling its action method.

Important

Always consult the platform-specific human interface guidelines before changing the default behavior of standard controls. For more information, see Human Interface Guidelines.

## See Also

### Simultaneous gestures

Preferring one gesture over another

Use a gesture recognizer delegate object to determine the order in which gestures are recognized in your views.

Allowing the simultaneous recognition of multiple gestures

Learn how to use a delegate object to allow detection of more than one gesture at a time.

