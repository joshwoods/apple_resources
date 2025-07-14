

- ActivityKit
- Activity
-  request(attributes:contentState:pushType:) Deprecated

Type Method

# request(attributes:contentState:pushType:)

Requests and starts a Live Activity.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
static func request(
    attributes: Attributes,
    contentState: Activity.ContentState,
    pushType: PushType? = nil
) throws -> Activity
```

Deprecated

Use request(attributes:content:pushType:) instead

## Parameters 

`attributes`  

A set of attributes that describe the Live Activity and its static content.

`contentState`  

A structure that describes the dynamic content of the Live Activity that changes over time.

`pushType`  

A value that indicates whether the Live Activity receives updates to its dynamic content with ActivityKit push notifications. Pass `nil` to start a Live Activity that only receives updates from the app with the update(_:) function. To start a Live Activity that receives updates to its dynamic content with ActivityKit push notifications in addition to the update(_:) function, pass token to this parameter.

## Return Value

The object that represents the started Live Activity.

## Discussion

Use this function to request and start a Live Activity from your app while it’s in the foreground. Note that you can’t do this while your app is in the background.

If your Live Activity displays image assets, the system requires them to use a resolution that’s smaller or equal to the size of the Live Activity presentation for a device. If you use an image asset that’s larger than the size of the Live Activity presentation, the system may fail to start the Live Activity. For information about the sizes of Live Activity presentations, see Human Interface Guidelines > Live Activities.

For additional information on starting a Live Activity, see Displaying live data with Live Activities.

Throws

ActivityAuthorizationError if the app can’t start a new Live Activity. For example, ActivityAuthorizationError.denied indicates that a person deactivated Live Activities for the app.

## See Also

### Deprecated symbols

var contentState: Activity&lt;Attributes>.ContentState

The dynamic content of a Live Activity.

Deprecated

func update(using: Activity&lt;Attributes>.ContentState, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

Deprecated

func end(using: Activity&lt;Attributes>.ContentState?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

Deprecated

var contentStateUpdates: Activity&lt;Attributes>.ContentStateUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

Deprecated

struct ContentStateUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

Deprecated

