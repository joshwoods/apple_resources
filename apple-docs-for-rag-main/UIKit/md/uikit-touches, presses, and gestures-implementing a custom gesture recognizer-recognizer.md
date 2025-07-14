

- UIKit
- Touches, presses, and gestures
-  Implementing a custom gesture recognizer 

# Implementing a custom gesture recognizer

Discover when and how to build your own gesture recognizers.

## Overview

When the built-in UIKit gesture recognizers don’t provide the behavior you want, you can define custom gesture recognizers. UIKit defines highly configurable gesture recognizers to handle touch sequences for taps, long presses, pans, swipes, rotations, and pinches. For other touch sequences, or to handle gestures that involve button presses, you can define a custom gesture recognizer.

You might also use a custom gesture recognizer to simplify the event-handling code in your app. For example, the Leveraging touch input for drawing apps sample uses a gesture recognizer to capture input and display it onscreen, as shown in the following image.

To define a custom gesture recognizer, subclass UIGestureRecognizer (or one of its subclasses). At the top of your source file, import the `UIGestureRecognizerSubclass.h` header file (for Objective-C) or the `UIKit.UIGestureRecognizerSubclass` module (for Swift), as shown in the following code. This file defines the methods and properties that you must override to implement your custom gesture recognizer.

- Swift
- Objective-C

```
import UIKit
import UIKit.UIGestureRecognizerSubclass
```

```
#import 
#import "UIGestureRecognizerSubclass.h"
```

In your custom subclass, implement whatever methods you need to process events. For example, if your gesture consists of touch events, implement the touchesBegan(_:with:), touchesMoved(_:with:), touchesEnded(_:with:), and touchesCancelled(_:with:) methods. Use incoming events to update the state property of your gesture recognizer. UIKit uses the gesture recognizer states to coordinate interactions with other objects in your interface.

## Topics

### Creating Custom Gesture Recognizers

About the Gesture Recognizer State Machine

Learn about the states and transitions of the state machine that underlies gesture recognizers.

Implementing a Discrete Gesture Recognizer

If your gesture involves a specific pattern of events, consider implementing a discrete gesture recognizer for it.

Implementing a Continuous Gesture Recognizer

For gestures that do not easily match a specific pattern, or when you want to use a gesture recognizer to gather touch input, create a continuous gesture recognizer.

## See Also

### Custom gestures

class UIGestureRecognizer

The base class for concrete gesture recognizers.

protocol UIGestureRecognizerDelegate

A set of methods implemented by the delegate of a gesture recognizer to fine-tune an app’s gesture-recognition behavior.

Supporting gesture interaction in your apps

Enrich your app’s user experience by supporting standard and custom gesture interaction.

