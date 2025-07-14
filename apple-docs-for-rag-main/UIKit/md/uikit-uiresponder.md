

- UIKit
-  UIResponder 

Class

# UIResponder

An abstract interface for responding to and handling events.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIResponder
```

## Mentioned in 

Using responders and the responder chain to handle events

Handling key presses made on a physical keyboard

## Overview

Responder objects — instances of UIResponder — constitute the event-handling backbone of a UIKit app. Many key objects are also responders, including the UIApplication object, UIViewController objects, and all UIView objects (which includes UIWindow). As events occur, UIKit dispatches them to your app’s responder objects for handling.

There are several kinds of events, including touch events, motion events, remote-control events, and press events. To handle a specific type of event, a responder must override the corresponding methods. For example, to handle touch events, a responder implements the touchesBegan(_:with:), touchesMoved(_:with:), touchesEnded(_:with:), and touchesCancelled(_:with:) methods. In the case of touches, the responder uses the event information provided by UIKit to track changes to those touches and to update the app’s interface appropriately.

In addition to handling events, UIKit responders also manage the forwarding of unhandled events to other parts of your app. If a given responder doesn’t handle an event, it forwards that event to the next event in the responder chain. UIKit manages the responder chain dynamically, using predefined rules to determine which object should be next to receive an event. For example, a view forwards events to its superview, and the root view of a hierarchy forwards events to its view controller.

Responders process UIEvent objects but can also accept custom input through an input view. The system’s keyboard is the most obvious example of an input view. When the user taps a UITextField and UITextView object onscreen, the view becomes the first responder and displays its input view, which is the system keyboard. Similarly, you can create custom input views and display them when other responders become active. To associate a custom input view with a responder, assign that view to the inputView property of the responder.

For information about responders and the responder chain, see Using responders and the responder chain to handle events.

## Topics

### Managing the responder chain

var next: UIResponder?

Returns the next responder in the responder chain, or `nil` if there’s no next responder.

var isFirstResponder: Bool

Returns a Boolean value indicating whether this object is the first responder.

var canBecomeFirstResponder: Bool

Returns a Boolean value indicating whether this object can become the first responder.

func becomeFirstResponder() -> Bool

Asks UIKit to make this object the first responder in its window.

var canResignFirstResponder: Bool

Returns a Boolean value indicating whether the responder is willing to relinquish first-responder status.

func resignFirstResponder() -> Bool

Notifies this object that it has been asked to relinquish its status as first responder in its window.

### Responding to touch events

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells this object that one or more new touches occurred in a view or window.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more touches associated with an event changed.

func touchesEnded(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more fingers are raised from a view or window.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when a system event (such as a system alert) cancels a touch sequence.

func touchesEstimatedPropertiesUpdated(Set&lt;UITouch>)

Tells the responder that updated values were received for previously estimated properties or that an update is no longer expected.

### Responding to motion events

func motionBegan(UIEvent.EventSubtype, with: UIEvent?)

Tells the responder that a motion event has begun.

func motionEnded(UIEvent.EventSubtype, with: UIEvent?)

Tells the responder that a motion event has ended.

func motionCancelled(UIEvent.EventSubtype, with: UIEvent?)

Tells the responder that a motion event has been canceled.

### Responding to press events

Generally, responders that handle press events should override all four of these methods.

func pressesBegan(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a physical button is first pressed.

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a value associated with a press has changed.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent?)

Tells the object when a button is released.

func pressesCancelled(Set&lt;UIPress>, with: UIPressesEvent?)

Tells this object when a system event (such as a low-memory warning) cancels a press event.

### Responding to remote-control events

func remoteControlReceived(with: UIEvent?)

Tells the object when a remote-control event is received.

### Managing input views

var inputView: UIView?

The custom input view to display when the responder becomes the first responder.

var inputViewController: UIInputViewController?

The custom input view controller to use when the responder becomes the first responder.

var inputAccessoryView: UIView?

The custom input accessory view to display when the responder becomes the first responder.

var inputAccessoryViewController: UIInputViewController?

The custom input accessory view controller to display when the responder becomes the first responder.

func reloadInputViews()

Updates the custom input and accessory views when the object is the first responder.

### Getting the undo manager

var undoManager: UndoManager?

Returns the nearest shared undo manager in the responder chain.

### Building and validating commands

func buildMenu(with: any UIMenuBuilder)

Asks the receiving responder to add and remove items from a menu system.

func validate(UICommand)

Asks the receiving responder to validate the command.

func canPerformAction(Selector, withSender: Any?) -> Bool

Requests the receiving responder to enable or disable the specified command in the user interface.

func target(forAction: Selector, withSender: Any?) -> Any?

Returns the target object that responds to an action.

### Accessing the available key commands

var keyCommands: [UIKeyCommand]?

The key commands that trigger actions on this responder.

### Managing the text input mode

var textInputMode: UITextInputMode?

The text input mode for this responder object.

var textInputContextIdentifier: String?

An identifier signifying that the responder should preserve its text input mode information.

class func clearTextInputContextIdentifier(String)

Clears text input mode information from the app’s user defaults.

var inputAssistantItem: UITextInputAssistantItem

The input assistant to use when configuring the keyboard’s shortcuts bar.

### Supporting user activities

var userActivity: NSUserActivity?

An object encapsulating a user activity supported by this responder.

func restoreUserActivityState(NSUserActivity)

Restores the state needed to continue the given user activity.

func updateUserActivityState(NSUserActivity)

Updates the state of the given user activity.

### Managing activity items

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

### Accessing the editing interaction

var editingInteractionConfiguration: UIEditingInteractionConfiguration

enum UIEditingInteractionConfiguration

### Capturing text from the camera

func captureTextFromCamera(Any?)

Starts scanning text using the device’s camera.

### Managing the Touch Bar

func makeTouchBar() -> NSTouchBar?

Asks the receiving responder to create and configure a Touch Bar object.

var touchBar: NSTouchBar?

The Touch Bar object for the responder.

### Constants

class let keyboardAnimationCurveUserInfoKey: String

A user info key to retrieve the animation curve that the system uses to animate the keyboard onto or off the screen.

class let keyboardAnimationDurationUserInfoKey: String

A user info key to retrieve the duration of the keyboard animation in seconds.

class let keyboardDidChangeFrameNotification: NSNotification.Name

A notification that posts immediately after a change in the keyboard’s frame.

class let keyboardDidHideNotification: NSNotification.Name

A notification that posts immediately after dismissing the keyboard.

class let keyboardDidShowNotification: NSNotification.Name

A notification that posts immediately after displaying the keyboard.

class let keyboardFrameBeginUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the beginning of its animation.

class let keyboardFrameEndUserInfoKey: String

A user info key to retrieve the keyboard’s frame at the end of its animation.

class let keyboardIsLocalUserInfoKey: String

A user info key to retrieve a Boolean value that indicates whether the keyboard belongs to the current app.

class let keyboardWillChangeFrameNotification: NSNotification.Name

A notification that posts immediately prior to a change in the keyboard’s frame.

class let keyboardWillHideNotification: NSNotification.Name

A notification that posts immediately prior to dismissing the keyboard.

class let keyboardWillShowNotification: NSNotification.Name

A notification that posts immediately prior to displaying the keyboard.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIAccessibilityElement
- UIApplication
- UIScene
- UIView
- UIViewController

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIUserActivityRestoring

## See Also

### Essentials

Using responders and the responder chain to handle events

Learn how to handle events that propagate through your app.

class UIEvent

An object that describes a single user interaction with your app.

