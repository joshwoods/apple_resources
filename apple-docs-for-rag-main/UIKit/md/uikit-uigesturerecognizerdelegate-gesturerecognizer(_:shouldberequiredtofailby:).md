

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldBeRequiredToFailBy:) 

Instance Method

# gestureRecognizer(\_:shouldBeRequiredToFailBy:)

Asks the delegate if a gesture recognizer should be required to fail by another gesture recognizer.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldBeRequiredToFailBy otherGestureRecognizer: UIGestureRecognizer
) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer. This is the object sending the message to the delegate.

`otherGestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer.

## Return Value

true to set up a dynamic failure requirement between `gestureRecognizer` and `otherGestureRecognizer`. The default implementation returns false—`gestureRecognizer` isn’t required to fail by `otherGestureRecognizer`.

## Mentioned in 

Preferring one gesture over another

## Discussion

This method is called once per attempt to recognize, so failure requirements can be determined lazily and may be set up between recognizers across view hierarchies. Note that returning true is guaranteed to set up the failure requirement; returning false, on the other hand, isn’t guaranteed to prevent or remove a failure requirement because `otherGestureRecognizer` might make itself a failure requirement by using its own subclass or delegate methods.

## See Also

### Setting up failure requirements

func gestureRecognizer(UIGestureRecognizer, shouldRequireFailureOf: UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should require another gesture recognizer to fail.

