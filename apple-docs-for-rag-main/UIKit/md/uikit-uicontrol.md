

- UIKit
-  UIControl 

Class

# UIControl

The base class for controls, which are visual elements that convey a specific action or intention in response to user interactions.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIControl
```

## Mentioned in 

Displaying and managing views with a view controller

## Overview

Controls implement elements such as buttons and sliders, which your app can use to facilitate navigation, gather user input, or manipulate content. Controls use the target-action mechanism to report user interactions to your app.

You don’t create instances of this class directly. The UIControl class is a subclassing point that you extend to implement custom controls. You can also subclass existing control classes to extend or modify their behaviors. For example, you might override the methods of this class to track touch events yourself or to determine when the state of the control changes.

A control’s state determines its appearance and its ability to support user interactions. Controls can be in one of several states, which the UIControl.State type defines. You can change the state of a control programmatically according to your app’s needs. For example, you might disable a control to prevent the user from interacting with it. User interactions can also change the state of a control.

### Respond to user interaction

The target-action mechanism simplifies the code that you write to use controls in your app. Instead of writing code to track touch events, you write action methods to respond to control-specific events. For example, you might write an action method that responds to changes in the value of a slider. The control handles all the work of tracking incoming touch events and determining when to call your methods.

When adding an action method to a control, you specify both the action method and an object that defines that method to the addTarget(_:action:for:) method. (You can also configure the target and action of a control in Interface Builder.) The target object can be any object, but it’s typically the view controller’s root view that contains the control. If you specify `nil` for the target object, the control searches the responder chain for an object that defines the specified action method.

The signature of an action method takes one of three forms. The `sender` parameter corresponds to the control that calls the action method, and the `event` parameter corresponds to the UIEvent object that triggered the control-related event.

- Swift
- Objective-C

```
@IBAction func doSomething()
@IBAction func doSomething(sender: UIButton)
@IBAction func doSomething(sender: UIButton, forEvent event: UIEvent)
```

```
- (IBAction)doSomething;
- (IBAction)doSomething:(id)sender;
- (IBAction)doSomething:(id)sender forEvent:(UIEvent*)event;
```

The system calls action methods when the user interacts with the control in specific ways. The UIControl.Event type defines the types of user interactions that a control can report and those interactions mostly correlate to specific touch events within the control. When configuring a control, you must specify which events trigger the calling of your method. For a button control, you might use the touchDown or touchUpInside event to trigger calls to your action method. For a slider, you might care only about changes to the slider’s value, so you might choose to attach your action method to valueChanged events.

When a control-specific event occurs, the control calls any associated action methods immediately. The current UIApplication object dispatches action methods and finds an appropriate object to handle the message, following the responder chain, if necessary. For more information about responders and the responder chain, see Event Handling Guide for UIKit Apps.

### Configure control attributes in Interface Builder

The following table lists the attributes for instances of the UIControl class.

| Attribute | Description |
|----|----|
| Alignment | The horizontal and vertical alignment of a control’s content. For controls that contain text or images, such as buttons and text fields, use these attributes to configure the position of that content within the control’s bounds.  These alignment options apply to the content of a control and not to the control itself. For information about how to align controls with respect to other controls and views, see Auto Layout Guide. |
| Content | The initial state of the control. Use the checkboxes to configure whether the control is in an enabled, selected, or highlighted state initially. |

### Support localization

Because UIControl is an abstract class, you don’t internationalize it specifically. However, you do internationalize the content of subclasses like UIButton. For information about internationalizing a specific control, see the reference for that control.

### Make controls accessible

Controls are accessible by default. To be useful, an accessible user interface element must provide accurate and helpful information about its screen position, name, behavior, value, and type. This is the information VoiceOver speaks to users. Users who are blind or have low vision can rely on VoiceOver to help them use their devices.

Controls support the following accessibility attributes:

- **Label.** A short, localized word or phrase that succinctly describes the control or view, but doesn’t identify the element’s type. Examples are *Add* and *Play*.

- **Traits.** A combination of one or more individual traits, each of which describes a single aspect of an element’s state, behavior, or usage. For example, you might use a combination of the Keyboard Key and the Selected traits to describe an element that behaves like a keyboard key and that’s in a selected state.

- **Hint.** A brief, localized phrase that describes the results of an action on an element. Examples are *Adds a title* and *Opens the shopping list*.

- **Frame.** The frame of the element in screen coordinates, which the `CGRect` structure specifies for an element’s screen location and size.

- **Value.** The current value of an element when the label doesn’t represent the value. For example, the label for a slider might be *Speed*, but its current value might be *50%*.

The `UIControl` class provides default content for the value and frame attributes. Many controls automatically enable additional specific traits as well. You can configure other accessibility attributes programmatically or with the Identity inspector in Interface Builder.

For more information about accessibility attributes, see Accessibility Programming Guide for iOS.

### Subclassing notes

Subclassing UIControl gives you access to the built-in target-action mechanism and simplified event-handling support. You can subclass existing controls and modify their behavior in one of two ways:

- Override the sendAction(_:to:for:) method of an existing subclass to observe or modify the dispatching of action methods to the control’s associated targets. You might use this method to modify the dispatch behavior for the specified object, selector, or event.

- Override the beginTracking(_:with:), continueTracking(_:with:), endTracking(_:with:), and cancelTracking(with:) methods to track touch events occurring in the control. You can use the tracking information to perform additional actions. Always use these methods to track touch events instead of the methods that the UIResponder class defines.

If you subclass UIControl directly, your subclass is responsible for setting up and managing your control’s visual appearance. Use the methods for tracking events to update your control’s state and to send an action when the control’s value changes.

## Topics

### Creating a control

convenience init(frame: CGRect, primaryAction: UIAction?)

Creates a control with the specified frame and primary action.

init(frame: CGRect)

Creates a control with the specified frame.

init?(coder: NSCoder)

Creates a control from data in an unarchiver.

### Managing state

var state: UIControl.State

The state of the control, specified as a bit mask value.

struct State

Constants describing the state of a control.

var isEnabled: Bool

A Boolean value indicating whether the control is in the enabled state.

var isSelected: Bool

A Boolean value indicating whether the control is in the selected state.

var isHighlighted: Bool

A Boolean value indicating whether the control draws a highlight.

### Specifying content alignment

var contentVerticalAlignment: UIControl.ContentVerticalAlignment

The vertical alignment of content within the control’s bounds.

enum ContentVerticalAlignment

Constants for specifying the vertical alignment of content (text and images) in a control.

var contentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment of content within the control’s bounds.

var effectiveContentHorizontalAlignment: UIControl.ContentHorizontalAlignment

The horizontal alignment currently in effect for the control.

enum ContentHorizontalAlignment

The horizontal alignment of content (text and images) within a control.

### Managing the control’s targets and actions

func addTarget(Any?, action: Selector, for: UIControl.Event)

Associates a target object and action method with the control.

func removeTarget(Any?, action: Selector?, for: UIControl.Event)

Stops the delivery of events to the specified target object.

var allTargets: Set&lt;AnyHashable>

Returns all target objects associated with the control.

func addAction(UIAction, for: UIControl.Event)

func removeAction(UIAction, for: UIControl.Event)

func removeAction(identifiedBy: UIAction.Identifier, for: UIControl.Event)

func actions(forTarget: Any?, forControlEvent: UIControl.Event) -> [String]?

Returns the actions performed on a target object when the specified event occurs.

var allControlEvents: UIControl.Event

Returns the events for which the control has associated actions.

func enumerateEventHandlers((UIAction?, (Any?, Selector)?, UIControl.Event, inout Bool) -> Void)

### Triggering actions

func performPrimaryAction()

Calls the method associated with the control’s primary action.

func sendAction(UIAction)

func sendAction(Selector, to: Any?, for: UIEvent?)

Calls the specified action method.

func sendActions(for: UIControl.Event)

Calls the action methods associated with the specified events.

### Tracking touches and redrawing controls

func beginTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event enters the control’s bounds.

func continueTracking(UITouch, with: UIEvent?) -> Bool

Notifies the control when a touch event for the control updates.

func endTracking(UITouch?, with: UIEvent?)

Notifies the control when a touch event associated with the control ends.

func cancelTracking(with: UIEvent?)

Notifies the control to cancel tracking related to the specified event.

var isTracking: Bool

A Boolean value that indicates whether the control is currently tracking touch events.

var isTouchInside: Bool

A Boolean value that indicates whether a tracked touch event is currently inside the control’s bounds.

### Managing context menus

Adding context menus in your app

Provide quick access to useful actions by adding context menus to your iOS app.

var contextMenuInteraction: UIContextMenuInteraction?

A context menu interaction for the control.

var isContextMenuInteractionEnabled: Bool

A Boolean value that determines whether the control enables its context menu interaction.

var showsMenuAsPrimaryAction: Bool

A Boolean value that determines whether the context menu interaction is the control’s primary action.

func contextMenuInteraction(UIContextMenuInteraction, configurationForMenuAtLocation: CGPoint) -> UIContextMenuConfiguration?

func contextMenuInteraction(UIContextMenuInteraction, previewForDismissingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, previewForHighlightingMenuWithConfiguration: UIContextMenuConfiguration) -> UITargetedPreview?

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

func menuAttachmentPoint(for: UIContextMenuConfiguration) -> CGPoint

### Showing tooltips

Show tooltips in your iPhone and iPad apps running on a Mac with Apple silicon, or your app built with Mac Catalyst.

var toolTip: String?

The default text to display in the control’s tooltip.

var toolTipInteraction: UIToolTipInteraction?

The tooltip interaction associated with the control.

### Constants

struct Event

Constants describing the types of events possible for controls.

### Instance Properties

var isSymbolAnimationEnabled: Bool

A Boolean value that indicates whether symbol effects animate.

## Relationships

### Inherits From

- UIView

### Inherited By

- UIButton
- UIColorWell
- UIDatePicker
- UIPageControl
- UIPasteControl
- UIRefreshControl
- UISegmentedControl
- UISlider
- UIStepper
- UISwitch
- UITextField

### Conforms To

- CALayerDelegate
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Controls

Responding to control-based events using target-action

Handle user input by connecting buttons, sliders, and other controls to your app’s code using the target-action design pattern.

class UIButton

A control that executes your custom code in response to user interactions.

class UIColorWell

A control that displays a color picker.

class UIDatePicker

A control for inputting date and time values.

class UIPageControl

A control that displays a horizontal series of dots, each of which corresponds to a page in the app’s document or other data-model entity.

class UISegmentedControl

A horizontal control that consists of multiple segments, each segment functioning as a discrete button.

class UISlider

A control for selecting a single value from a continuous range of values.

class UIStepper

A control for incrementing or decrementing a value.

class UISwitch

A control that offers a binary choice, such as on/off.

