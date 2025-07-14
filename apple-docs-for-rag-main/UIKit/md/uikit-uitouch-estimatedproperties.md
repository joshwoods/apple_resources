

- UIKit
- UITouch
-  estimatedProperties 

Instance Property

# estimatedProperties

A set of touch properties whose values contain only estimates.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var estimatedProperties: UITouch.Properties { get }
```

## Discussion

This property contains a bitmask of constants indicating which touch properties could not be reported immediately. For example, Apple Pencil records the force of a touch, but must transmit that information over the air to the underlying iPad. The delay incurred by transmitting the data may cause the information to be received after the touch has been reported to your app.

Values in this property are not guaranteed to be updated later. For a list of properties whose values are expected to be updated, see estimatedPropertiesExpectingUpdates.

## See Also

### Managing estimated touch attributes

var estimatedPropertiesExpectingUpdates: UITouch.Properties

The set of touch properties for which updated values are expected in the future.

struct Properties

A bit mask of touch properties that may get updated.

var estimationUpdateIndex: NSNumber?

An index number that lets you correlate an updated touch with the original touch.

