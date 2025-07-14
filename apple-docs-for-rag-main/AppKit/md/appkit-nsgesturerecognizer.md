

- AppKit
-  NSGestureRecognizer 

Class

# NSGestureRecognizer

An object that monitors events and calls its action method when a predefined sequence of events occur.

macOS 10.10+

``` source
@MainActor
class NSGestureRecognizer
```

## Overview

A gesture recognizer might recognize a single click, a click and drag, or a sequence of events that imply rotation. You do not create instances of this class directly. This class is an abstract base class that defines the common behavior for all gesture recognizers. When using a gesture recognizer in your app, create an instance of one of the concrete subclasses.

The concrete subclasses of NSGestureRecognizer are the following:

- NSClickGestureRecognizer

- NSMagnificationGestureRecognizer

- NSPanGestureRecognizer

- NSPressGestureRecognizer

- NSRotationGestureRecognizer

A gesture recognizer operates on events in a specific view (or in any of that view’s subviews). After creating a gesture recognizer, attach it to one of your views using the addGestureRecognizer(_:) method. Events received by your app are forwarded automatically to any relevant gesture recognizers before they are sent to the corresponding view. The gesture recognizer can delay the further progression of the events until recognition is complete or allow the events to be delivered normally.

A gesture recognizer can detect gestures that are either discrete or continuous in nature. A click gesture is discrete because it involves a mouse-down and mouse-up event without any mouse movements in between. By contrast, a pan or rotation gesture is continuous because it involves tracking mouse movements over a period of time.

During the gesture recognition process, a gesture recognizer calls the action method of its associated target object to report the state of the recognition process. For discrete gestures, the action method is typically called only once when the gesture is recognized. For continuous gestures, it may be called multiple times depending on the current state of the gesture recognizer. In that situation, you can use your action method to perform appropriate tasks, such as creating animations for any mouse-related movements, in addition to handling the final results of the gesture recognition process.

A gesture recognizer has only one action method and one target object, and the method must conform to one of the following signatures:

- Swift
- Objective-C

```
func handleGesture() { }
func handleGesture(gestureRecognizer: NSGestureRecognizer) { }
```

```
- (void)handleGesture;
- (void)handleGesture:(NSGestureRecognizer *)gestureRecognizer;
```

When your code needs additional information about the particulars of a gesture, define your action method to include the gesture recognizer parameter. You almost always want the gesture recognizer object when handling continuous gestures. For example, for a rotation gesture, you would use the gesture recognizer object to get the updated rotation value. You can also use the gesture recognizer object to get the location of where the gesture occurred.

### State Transitions

Gesture recognizers operate within a predefined state machine, transitioning from state to state as they handle events. All gesture recognizers begin in the Possible (NSGestureRecognizer.State.possible) state, but the possible transitions differ for continuous and discrete gestures.

Discrete gestures transition from the Possible state directly to the Recognized (recognized) or Failed (NSGestureRecognizer.State.failed) state, depending on whether they successfully interpret the gesture. When a discrete gesture recognizer transitions to the Recognized state, it calls the action method of its target object.

For continuous gestures, the state transitions are as follows:

- Possible —\> Began —\> \[Changed\] —\> Cancelled

- Possible —\> Began —\> \[Changed\] —\> Ended

The Changed state is optional and may occur multiple times before the Cancelled or Ended state is reached. Many state transitions cause the gesture recognizer to call its action method. Setting the state property to NSGestureRecognizer.State.changed while monitoring events also calls the action method. You can use these calls to update the state of your app or update any custom animations.

For a list of possible states, see the constants in NSGestureRecognizer.State.

### Subclassing Notes

You may create a subclass of `NSGestureRecognizer` that recognizes a distinctive gesture—for example, a “check mark” gesture. A custom gesture recognizer implements any appropriate event-related methods to detect its gesture along with a few other methods for managing state information.

All gesture recognizers must update the value in the state property at appropriate times. Specifically, you must update it for all state transitions. For more information about the possible state transitions of a gesture recognizer, see State Transitions.

Note

NSGestureRecognizer does not support handing off event tracking to other non-gesture recognizer mechanisms (for example drag and drop and pop-up menus).

#### Methods to Override

When creating your own gesture recognizer subclass:

- Implement the reset() method and any other relevant methods in Methods for Subclasses.

- Override the location(in:) method as needed to specify an appropriate point for your gesture.

AppKit waits for a mouse-down event, magnify event, or rotation event to occur before starting the gesture recognition process. A gesture recognizer that used only key-down events to recognize its gesture would not have its keyDown(with:) method called until a mouse-down, magnify, or rotation event started the recognition process.

#### Alternatives to Subclassing

The `NSGestureRecognizer` class defines the common behaviors that can be configured for all concrete gesture recognizers. It also supports a delegate—an object that adopts the NSGestureRecognizerDelegate protocol—for handling finer-grained customization of some behaviors without the need for subclassing. For example, you can use the delegate to create dependencies between specific gesture recognizer objects.

For more information about using the delegate to control the behavior of your gesture recognizers, see NSGestureRecognizerDelegate.

## Topics

### Initializing a Gesture Recognizer

init(target: Any?, action: Selector?)

Initializes the gesture recognizer with the specified target and action information.

### Accessing the Target and Action

var action: Selector?

The action method to call when the gesture is recognized.

var target: AnyObject?

The object that implements the action method.

### Getting the Location of Events

func location(in: NSView?) -> NSPoint

Returns the point computed as the location of the gesture.

### Accessing the Recognizer’s State

var state: NSGestureRecognizer.State

The current state of the gesture recognizer.

var view: NSView?

The view to which the gesture recognizer is attached.

var isEnabled: Bool

A Boolean value indicating whether the gesture recognizer is able to handle events.

### Delaying Events

var delaysPrimaryMouseButtonEvents: Bool

A Boolean value that indicates whether primary mouse button events are delivered only after gesture recognition fails.

var delaysSecondaryMouseButtonEvents: Bool

A Boolean value that indicates whether secondary mouse button events are delivered only after gesture recognition fails.

var delaysOtherMouseButtonEvents: Bool

A Boolean value that indicates whether other mouse button events are delivered only after gesture recognition fails.

var delaysKeyEvents: Bool

A Boolean value that indicates whether key events are delivered only after gesture recognition fails.

var delaysMagnificationEvents: Bool

A Boolean value that indicates whether magnification events are delivered only after gesture recognition fails.

var delaysRotationEvents: Bool

A Boolean value that indicates whether rotation events are delivered only after gesture recognition fails.

### Accessing the Delegate

var delegate: (any NSGestureRecognizerDelegate)?

The delegate of the gesture recognizer.

### Methods for Subclasses

func reset()

Overridden to reset the internal state of the gesture recognizer when an attempt completes.

func mouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed the left mouse button.

func mouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with the left button pressed.

func mouseUp(with: NSEvent)

Informs the gesture recognizer that the user released the left mouse button.

func otherMouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed a mouse button other than the left or right one.

func otherMouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with a button other than the left or right one pressed.

func otherMouseUp(with: NSEvent)

Informs the gesture recognizer that the user released a mouse button other than the left or right one.

func rightMouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed the right mouse button.

func rightMouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with the right button pressed.

func rightMouseUp(with: NSEvent)

Informs the gesture recognizer that the user released the right mouse button.

func magnify(with: NSEvent)

Informs the gesture recognizer that the user is performing a pinch gesture.

func rotate(with: NSEvent)

Informs the gesture recognizer that the user is performing a rotation gesture.

func canBePrevented(by: NSGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer can prevent the current object from recognizing a gesture.

func canPrevent(NSGestureRecognizer) -> Bool

Overridden to indicate that the current object can prevent the specified gesture recognizer from recognizing its gesture.

func shouldBeRequiredToFail(by: NSGestureRecognizer) -> Bool

Overridden to indicate that the current object must fail before the specified gesture recognizer begins recognizing its gesture.

func shouldRequireFailure(of: NSGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer must fail before the current object begins recognizing its gesture.

func keyDown(with: NSEvent)

Informs the gesture recognizer that the user has pressed a key.

func keyUp(with: NSEvent)

Informs the gesture recognizer that the user released a key.

func tabletPoint(with: NSEvent)

Informs the user that a tablet-point event occurred.

func flagsChanged(with: NSEvent)

Informs the current object that the user pressed or released a modifier key (Shift, Control, and so on).

func pressureChange(with: NSEvent)

Informs the current object that a pressure change occurred on a system that supports pressure sensitivity.

### Configuring Pressure

var pressureConfiguration: NSPressureConfiguration

Configures the behavior and progression of the Force Touch trackpad when responding to recognized pressure gestures.

### Constants

enum State

The current state of the gesture recognizer.

### Initializers

init?(coder: NSCoder)

### Instance Properties

var allowedTouchTypes: NSTouch.TouchTypeMask

### Instance Methods

func touchesBegan(with: NSEvent)

Called when one or more fingers first make contact with an NSTouchBar instance on the Touch Bar.

func touchesCancelled(with: NSEvent)

Called when a system event, such as a low-memory warning, cancels an in-progress touch event in an NSTouchBar object.

func touchesEnded(with: NSEvent)

Called when one or more fingers are removed from contact with an NSTouchBar instance on the Touch Bar.

func touchesMoved(with: NSEvent)

Called when one or more fingers, associated with an in-progress event, move within an NSTouchBar instance on the Touch Bar.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSClickGestureRecognizer
- NSMagnificationGestureRecognizer
- NSPanGestureRecognizer
- NSPressGestureRecognizer
- NSRotationGestureRecognizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Custom Gestures

protocol NSGestureRecognizerDelegate

A set of methods for fine-tuning a gesture recognizer’s behavior.

