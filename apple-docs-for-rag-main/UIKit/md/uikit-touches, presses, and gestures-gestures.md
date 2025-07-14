

- UIKit
-  Touches, presses, and gestures 

API Collection

# Touches, presses, and gestures

Encapsulate your app’s event-handling logic in gesture recognizers so that you can reuse that code throughout your app.

## Overview

If you build your apps using standard UIKit views and controls, UIKit automatically handles touch events (including Multitouch events) for you. However, if you use custom views to display your content, you must handle all touch events that occur in your views. There are two ways to handle touch events yourself.

- Use gesture recognizers to track the touches; see Handling UIKit gestures.

- Track the touches directly in your UIView subclass; see Handling touches in your view.

## Topics

### Essentials

Using responders and the responder chain to handle events

Learn how to handle events that propagate through your app.

class UIResponder

An abstract interface for responding to and handling events.

class UIEvent

An object that describes a single user interaction with your app.

### Touches

Handling touches in your view

Use touch events directly on a view subclass if touch handling is intricately linked to the view’s content.

Handling input from Apple Pencil

Learn how to detect and respond to touches from Apple Pencil.

Tracking the force of 3D Touch events

Manipulate your content based on the force of touches.

Illustrating the force, altitude, and azimuth properties of touch input

Capture Apple Pencil and touch input in views.

Leveraging touch input for drawing apps

Capture touches as a series of strokes and render them efficiently on a drawing canvas.

class UITouch

An object representing the location, size, movement, and force of a touch occurring on the screen.

### Button presses

class UIPress

An object that represents the presence or movement of a button press on the screen for a particular event.

class UIPressesEvent

An event that describes the state of a set of physical buttons that are available to the device, such as those on an associated remote or game controller.

### Standard gestures

Handling UIKit gestures

Use gesture recognizers to simplify touch handling and create a consistent user experience.

Coordinating multiple gesture recognizers

Discover how to use multiple gesture recognizers on the same view.

Adopting hover support for Apple Pencil

Enhance user feedback for your iPadOS app with a hover preview for Apple Pencil input.

Supporting gesture interaction in your apps

Enrich your app’s user experience by supporting standard and custom gesture interaction.

class UIHoverGestureRecognizer

A continuous gesture recognizer that interprets pointer movement over a view.

class UILongPressGestureRecognizer

A continuous gesture recognizer that interprets long-press gestures.

class UIPanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures.

class UIPinchGestureRecognizer

A continuous gesture recognizer that interprets pinching gestures involving two touches.

class UIRotationGestureRecognizer

A continuous gesture recognizer that interprets rotation gestures involving two touches.

class UIScreenEdgePanGestureRecognizer

A continuous gesture recognizer that interprets panning gestures that start near an edge of the screen.

class UISwipeGestureRecognizer

A discrete gesture recognizer that interprets swiping gestures in one or more directions.

class UITapGestureRecognizer

A discrete gesture recognizer that interprets single or multiple taps.

### Custom gestures

Implementing a custom gesture recognizer

Discover when and how to build your own gesture recognizers.

class UIGestureRecognizer

The base class for concrete gesture recognizers.

protocol UIGestureRecognizerDelegate

A set of methods implemented by the delegate of a gesture recognizer to fine-tune an app’s gesture-recognition behavior.

Supporting gesture interaction in your apps

Enrich your app’s user experience by supporting standard and custom gesture interaction.

### 3D Touch interactions

class UIPreviewInteraction

A class that registers a view to provide a custom user experience in response to 3D Touch interactions.

protocol UIPreviewInteractionDelegate

A set of methods for communicating the progress of a preview interaction.

protocol UIPreviewActionItem

A set of methods that defines the styles you can apply to peek quick actions and peek quick action groups, and defines a read-only accessor for the user-visible title of a peek quick action.

## See Also

### User interactions

Menus and shortcuts

Simplify interactions with your app using menu systems, contextual menus, Home Screen quick actions, and keyboard shortcuts.

Drag and drop

Bring drag and drop to your app by using interaction APIs with your views.

Pointer interactions

Support pointer interactions in your custom controls and views.

Apple Pencil interactions

Handle user interactions like double tap and squeeze on Apple Pencil.

Focus-based navigation

Navigate the interface of your UIKit app using a remote, game controller, or keyboard.

Accessibility for UIKit

Make your UIKit apps accessible to everyone who uses iOS and tvOS.

