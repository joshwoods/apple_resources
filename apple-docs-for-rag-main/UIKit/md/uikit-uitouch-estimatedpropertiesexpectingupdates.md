

- UIKit
- UITouch
-  estimatedPropertiesExpectingUpdates 

Instance Property

# estimatedPropertiesExpectingUpdates

The set of touch properties for which updated values are expected in the future.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var estimatedPropertiesExpectingUpdates: UITouch.Properties { get }
```

## Discussion

This property contains a bitmask of constants indicating which touch properties could not be reported immediately, and for which an update is expected later. When this property contains a non empty set, you can expect UIKit to call the touchesEstimatedPropertiesUpdated(_:) method of your responder or gesture recognizer at a later time with the updated values for the given properties. Attach the value in the estimationUpdateIndex property to your app’s copy of the touch data. When UIKit calls the touchesEstimatedPropertiesUpdated(_:) method later, use the estimation update index of the new touch to locate and update your app’s copy of the touch data.

When this property contains an empty set, no more updates are expected. In that scenario, the estimated or updated value is the final value.

## See Also

### Managing estimated touch attributes

var estimatedProperties: UITouch.Properties

A set of touch properties whose values contain only estimates.

struct Properties

A bit mask of touch properties that may get updated.

var estimationUpdateIndex: NSNumber?

An index number that lets you correlate an updated touch with the original touch.

