

- UIKit
- UIResponder
-  touchesEstimatedPropertiesUpdated(\_:) 

Instance Method

# touchesEstimatedPropertiesUpdated(\_:)

Tells the responder that updated values were received for previously estimated properties or that an update is no longer expected.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func touchesEstimatedPropertiesUpdated(_ touches: Set)
```

## Parameters 

`touches`  

The array of UITouch objects containing the updated properties. In each touch object, UIKit updates the estimatedPropertiesExpectingUpdates property by removing the bit flag for each property that was updated.

## Discussion

When UIKit is unable to report actual values for a touch, it delivers estimates for the values and sets the appropriate bits in the estimatedProperties and estimatedPropertiesExpectingUpdates properties of the UITouch object. When updates are received for items in the estimatedPropertiesExpectingUpdates property, UIKit calls this method to deliver those updates. UIKit also calls this method if one or more updates are no longer expected. You use this method to update your app’s internal data structures with the new values provided by UIKit.

In your implementation of this method, use the estimationUpdateIndex property of a UITouch object in the `touches` parameter to locate the original data in your app. Upon locating the data, apply the new values from the touch object to it. You can determine which touch properties were updated by checking the estimatedPropertiesExpectingUpdates bit mask of the touch object; updated properties are no longer included in the bit mask.

Touch-related properties may remain estimated because of hardware considerations. For example, sensors may not be able to ascertain the exact altitude or azimuth of Apple Pencil when it’s near the edges of the screen. In those cases, the estimatedProperties property continues to store the list of properties whose values are only estimates.

## See Also

### Responding to touch events

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells this object that one or more new touches occurred in a view or window.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more touches associated with an event changed.

func touchesEnded(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more fingers are raised from a view or window.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when a system event (such as a system alert) cancels a touch sequence.

