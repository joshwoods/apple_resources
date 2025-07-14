

- ActivityKit
- Activity
-  request(attributes:content:pushType:) 

Type Method

# request(attributes:content:pushType:)

Requests and starts a Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
static func request(
    attributes: Attributes,
    content: ActivityContent.ContentState>,
    pushType: PushType? = nil
) throws -> Activity
```

## Parameters 

`attributes`  

A set of attributes that describe the Live Activity and its static content.

`content`  

A structure that describes the dynamic content of the Live Activity that changes over time.

`pushType`  

A value that indicates whether the Live Activity receives updates to its dynamic content with ActivityKit push notifications. Pass `nil` to start a Live Activity that only receives updates from the app with the update(_:) function. To start a Live Activity that receives updates to its dynamic content with ActivityKit push notifications in addition to the update(_:) function, pass token to this parameter.

## Return Value

The object that represents the Live Activity you started.

## Mentioned in 

Starting and updating Live Activities with ActivityKit push notifications

Displaying live data with Live Activities

## Discussion

Use this function to request and start a Live Activity from your app while it’s in the foreground. Note that you can’t do this while your app is in the background.

If your Live Activity displays image assets, the system requires them to use a resolution that’s smaller or equal to the size of the Live Activity presentation for a device. If you use an image asset that’s larger than the size of the Live Activity presentation, the system may fail to start the Live Activity. For information about the sizes of Live Activity presentations, see Human Interface Guidelines > Live Activities.

For additional information on starting a Live Activity, see Displaying live data with Live Activities.

Throws

ActivityAuthorizationError if the app can’t start a new Live Activity. For example, ActivityAuthorizationError.denied indicates that the person deactivated Live Activities for the app.

## See Also

### Starting a Live Activity

let attributes: Attributes

A set of attributes that describe a Live Activity and its content.

protocol ActivityAttributes

The protocol you implement to describe the content of a Live Activity.

enum ActivityStyle

var content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>

The dynamic content of a Live Activity.

struct ActivityContent

A structure that describes the state and configuration of a Live Activity.

typealias ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

struct PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

enum ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

