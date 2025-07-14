

- UIKit
- Touches, presses, and gestures
-  Handling touches in your view 

# Handling touches in your view

Use touch events directly on a view subclass if touch handling is intricately linked to the view’s content.

## Overview

If you don’t plan to use gesture recognizers with a custom view, you can handle touch events directly from the view itself. Because views are responders, they can handle Multi-Touch events and many other types of events. When UIKit determines that a touch event occurred in a view, it calls the view’s touchesBegan(_:with:), touchesMoved(_:with:), or touchesEnded(_:with:) method. You can override these methods in your custom views and use them to provide a response to touch events.

The methods you override in your views (or in any responder) to handle touches correspond to different phases of the touch event-handling process. For example, the following image illustrates the different phases of a touch event. When a finger (or Apple Pencil) touches the screen, UIKit creates a UITouch object, sets the touch location to the appropriate point, and sets its phase property to UITouch.Phase.began. When the same finger moves around the screen, UIKit updates the touch location and changes the phase property of the touch object to UITouch.Phase.moved. When the user lifts the finger from the screen, UIKit changes the phase property to UITouch.Phase.ended and the touch sequence ends.

Similarly, the system may cancel an ongoing touch sequence at any time; for example, when an incoming phone call interrupts the app. When it does, UIKit notifies your view by calling the touchesCancelled(_:with:) method. You use that method to perform any needed cleanup of your view’s data structures.

UIKit creates a new UITouch object for each new finger that touches the screen. The touches themselves are delivered with the current UIEvent object. UIKit distinguishes between touches originating from a finger and from Apple Pencil, and you can treat each of them differently.

Important

In its default configuration, a view receives only the first UITouch object associated with an event, even if more than one finger is touching the view. To receive the additional touches, you must set the view’s isMultipleTouchEnabled property to true. You can also configure this property in Interface Builder using the Attributes inspector.

## Topics

### Advanced touch handling

Implementing a Multi-Touch app

Learn how to create a simple app that handles multitouch input.

Getting high-fidelity input with coalesced touches

Learn how to support high-precision touches in your app.

Minimizing latency with predicted touches

Create a smooth and responsive drawing experience using UIKit’s predictions for touch locations.

## See Also

### Touches

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

