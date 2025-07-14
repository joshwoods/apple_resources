

- UIKit
-  UIGestureRecognizerDelegate 

Protocol

# UIGestureRecognizerDelegate

A set of methods implemented by the delegate of a gesture recognizer to fine-tune an app’s gesture-recognition behavior.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UIGestureRecognizerDelegate : NSObjectProtocol
```

## Mentioned in 

Preferring one gesture over another

## Overview

The delegates receive messages from a gesture recognizer, and their responses to these messages enable them to affect the operation of the gesture recognizer or to specify a relationship between it and another gesture recognizer, such as allowing simultaneous recognition or setting up a dynamic failure requirement.

An example of a situation where dynamic failure requirements are useful is in an app that attaches a screen-edge pan gesture recognizer to a view. In this case, you might want all other relevant gesture recognizers associated with that view’s subtree to require the screen-edge gesture recognizer to fail so you can prevent any graphical glitches that might occur when the other recognizers get canceled after starting the recognition process. To do this, you could use code similar to the following:

- Swift
- Objective-C

```
let myScreenEdgePanGestureRecognizer = UIScreenEdgePanGestureRecognizer(target: self, action:#selector(handleScreenEdgePan))
myScreenEdgePanGestureRecognizer.delegate = self
    // Configure the gesture recognizer and attach it to the view.

...

func gestureRecognizer(_ gestureRecognizer: UIGestureRecognizer, shouldBeRequiredToFailBy otherGestureRecognizer: UIGestureRecognizer) -> Bool {
    guard let myView = myScreenEdgePanGestureRecognizer.view,
          let otherView = otherGestureRecognizer.view else { return false }

    return gestureRecognizer == myScreenEdgePanGestureRecognizer &&
           otherView.isDescendant(of: myView)}
```

```
UIScreenEdgePanGestureRecognizer *myScreenEdgePanGestureRecognizer;
...
myScreenEdgePanGestureRecognizer = [[UIScreenEdgePanGestureRecognizer alloc] initWithTarget:self action:@selector(handleScreenEdgePan:)];
myScreenEdgePanGestureRecognizer.delegate = self;
// Configure the gesture recognizer and attach it to the view.
...
 - (BOOL)gestureRecognizer:(UIGestureRecognizer *)gestureRecognizer shouldBeRequiredToFailByGestureRecognizer:(UIGestureRecognizer *)otherGestureRecognizer {
    BOOL result = NO;
    if ((gestureRecognizer == myScreenEdgePanGestureRecognizer) && [[otherGestureRecognizer view] isDescendantOfView:[gestureRecognizer view]]) {
        result = YES;
    }
    return result;
 }
```

## Topics

### Regulating gesture recognition

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should begin interpreting touches.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UITouch) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIPress) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a press.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIEvent) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch or press event.

### Controlling simultaneous gesture recognition

func gestureRecognizer(UIGestureRecognizer, shouldRecognizeSimultaneouslyWith: UIGestureRecognizer) -> Bool

Asks the delegate if two gesture recognizers should be allowed to recognize gestures simultaneously.

### Setting up failure requirements

func gestureRecognizer(UIGestureRecognizer, shouldRequireFailureOf: UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should require another gesture recognizer to fail.

func gestureRecognizer(UIGestureRecognizer, shouldBeRequiredToFailBy: UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should be required to fail by another gesture recognizer.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UITableViewCell

## See Also

### Custom gestures

Implementing a custom gesture recognizer

Discover when and how to build your own gesture recognizers.

class UIGestureRecognizer

The base class for concrete gesture recognizers.

Supporting gesture interaction in your apps

Enrich your app’s user experience by supporting standard and custom gesture interaction.

