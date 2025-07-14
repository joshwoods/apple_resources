

- UIKit
- UIActivityViewController
-  init(activityItems:applicationActivities:) 

Initializer

# init(activityItems:applicationActivities:)

Initializes a new activity view controller object that acts on the specified data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    activityItems: [Any],
    applicationActivities: [UIActivity]?
)
```

## Parameters 

`activityItems`  

The array of data objects on which to perform the activity. The type of objects in the array is variable and dependent on the data your application manages. For example, the data might consist of one or more string or image objects representing the currently selected content.

Instead of actual data objects, the objects in this array can be objects that adopt the UIActivityItemSource protocol, such as UIActivityItemProvider objects. Source and provider objects act as proxies for the corresponding data in situations where you do not want to provide that data until it is needed. Note that you should not reuse an activity view controller object that includes a UIActivityItemProvider object in its `activityItems` array.

This array must not be `nil` and must contain at least one object.

`applicationActivities`  

An array of UIActivity objects representing the custom services that your application supports. This parameter may be `nil`.

## Return Value

The activity view controller to present.

## Discussion

It is your responsibility to present and dismiss the view controller using the appropriate means for the given device idiom. On iPad, you must present the view controller in a popover. On other devices, you must present it modally.

## See Also

### Initializing the activity view controller

convenience init(activityItemsConfiguration: any UIActivityItemsConfigurationReading)

Initializes a new activity view controller object that acts on the specified configuration.

class UIActivityItemsConfiguration

A configuration that allows a responder to export data through a variety of interactions.

protocol UIActivityItemsConfigurationReading

A set of methods adopted by an object so that the object can act as an activity items configuration.

