

- UIKit
- Touches, presses, and gestures
- Handling UIKit gestures
-  Handling tap gestures 

Article

# Handling tap gestures

Use brief taps on the screen to implement button-like interactions with your content.

## Overview

Tap gestures detect one or more fingers touching the screen briefly. The fingers involved in these gestures must not move significantly from the initial touch points, and you can configure the number of times the fingers must touch the screen. For example, you might configure tap gesture recognizers to detect single taps, double taps, or triple taps.

You can attach a gesture recognizer in one of these ways:

- Programmatically. Call the addGestureRecognizer(_:) method of your view.

- In Interface Builder. Drag the appropriate object from the library and drop it onto your view.

A UITapGestureRecognizer object provides event handling capabilities similar to those of a button — it detects a tap in its view and reports that tap to your action method. Tap gestures are discrete, so your action method is called only when the tap gesture is recognized successfully. You can configure a tap gesture recognizer to require any number of taps — for example, single taps or double taps — before your action method is called.

The following code shows an action method that responds to a successful tap in a view by animating that view to a new location. Always check the gesture recognizer’s state property before taking any actions, even for a discrete gesture recognizer.

```
@IBAction func tapPiece(_ gestureRecognizer : UITapGestureRecognizer ) {
   guard gestureRecognizer.view != nil else { return }

   if gestureRecognizer.state == .ended {      // Move the view down and to the right when tapped.
      let animator = UIViewPropertyAnimator(duration: 0.2, curve: .easeInOut, animations: {
         gestureRecognizer.view!.center.x += 100
         gestureRecognizer.view!.center.y += 100
      })
      animator.startAnimation()
   }}

```

If the code for your tap gesture recognizer isn’t called, check to see if the following conditions are true, and make corrections as needed:

- The isUserInteractionEnabled property of the view is set to true. Image views and labels set this property to false by default.

- The number of taps was equal to the number specified in the numberOfTapsRequired property.

- The number of fingers was equal to the number specified in the numberOfTouchesRequired property.

## See Also

### Gestures

Handling long-press gestures

Detect extended duration taps on the screen, and use them to reveal contextually relevant content.

Handling pan gestures

Trace the movement of fingers around the screen, and apply that movement to your content.

Handling swipe gestures

Detect a horizontal or vertical swipe motion on the screen, and use it to trigger navigation through your content.

Handling pinch gestures

Track the distance between two fingers and use that information to scale or zoom your content.

Handling rotation gestures

Measure the relative rotation of two fingers on the screen, and use that motion to rotate your content.

