

- Core Location
-  Creating a location push service extension 

Article

# Creating a location push service extension

Add and configure an extension to enable your location-sharing app to access a user’s location in response to a request from another user.

## Overview

The Location Push Service Extension, available starting in iOS 15, is a power efficient way to query locations on iOS or iPadOS devices, even when your app isn’t running.

When your app includes a Location Push Service Extension, the system activates the extension when it receives an Apple Push Notification service (APNs) `location` push from your server. Your app must ask for and receive Always authorization (CLAuthorizationStatus.authorizedAlways) from the user before the extension can function. For more information about requesting Always authorization, see Requesting authorization to use location services and requestAlwaysAuthorization().

With the user’s authorization, the extension can query the user’s location and process it according to your app’s purpose. Your server sends requests with the `location` push type to APNs. For more information about sending requests to APNs, see Sending notification requests to APNs.

Important

To use the Location Push Service Extension, your app must have the com.apple.developer.location.push entitlement. Request this entitlement before implementing this service extension. To apply for the entitlement, log in to your developer account with an Account Holder role and fill out the request form.

### Configure Your Xcode Project

To include Location Push Service Extension in your app, use Xcode 13 or later. Configure the following entitlements, capabilities, and keys for your Xcode project:

1.  Set the Location Push Server Extension entitlement key (com.apple.developer.location.push).

2.  Enable your app to receive Apple Push Notification service (APNs) pushes by adding the Push Notifications capability. For more information, see Registering your app with APNs.

3.  Configure the purpose strings your app provides for the location service authorization prompts. For more information, see Requesting authorization to use location services.

### Add a Location Push Service Extension Target

Add a new target using the Location Push Service Extension template.

1.  Open your iOS app project in Xcode.

2.  Choose File \> New \> Target.

3.  Select Location Push Service Extension from the iOS Application Extension group.

4.  Click Next.

5.  Specify the name of your extension and configure the language and other options.

6.  Click Finish.

Xcode creates a subclass of CLLocationPushServiceExtension to get you started.

### Implement Location Push Functionality

To support location push functionality, implement the following code in your extension, app, and server:

1.  In your service extension, implement the CLLocationPushServiceExtension protocol.

2.  In your service extension, implement the locationManager(_:didUpdateLocations:) method to handle the result of the location request, and process the location data received.

3.  In your app, call startMonitoringLocationPushes(completion:) to receive an APNs token as `Data`, and send it to your server. Your server uses this token when it creates APNs pushes.

4.  From your server, request location information by sending a `location` push request to APNs.

If the user authorized your app with Always authorization (CLAuthorizationStatus.authorizedAlways), the system activates the service extension when it receives a `location` push, and calls didReceiveLocationPushPayload(_:completion:). Your app should ask the user for Always authorization at an appropriate time.

Important

Protecting user privacy is important when handling location data. End-to-end encryption provides enhanced security if your app moves location data off the user’s device, including transmitting it to a server or to another user. For more information, see Protecting the User’s Privacy.

### Send Location Push Requests From Your Server

When a user requests the location of another user, your app sends the request to your server, which sends a location push request to APNs. Ensure that your APNs `POST` request contains the following fields for a `location` push type:

`method`  
(Required) The value is `POST`.

`path`  
(Required) The path to the device token. The value of this header is `/3/device/`, where `` is the hexadecimal identifier of the user’s device. Your app receives the token when it calls startMonitoringLocationPushes(completion:) to start monitoring location pushes.

`authorization`  
(Required for token-based authentication) The value of this header is `bearer `, where `` is the encrypted token that authorizes you to send notifications for the specified topic. For more information, see Establishing a token-based connection to APNs.

`apns-topic`  
The topic is your app’s bundle ID with the suffix `".location-query"`.

`apns-push-type`  
(Recommended) The value of this header is `location`.

`apns-priority`  
The priority of the notification. If you omit this header, APNs sets the notification priority to `10`. If a user initiates the location query, set this header to `10`. If your app’s server initiates the location query (for example, on a periodic interval) set this header to `5` to send the notification based on power considerations on the user’s device.

For more information about sending APNs requests and using command-line tools to do so, see Sending notification requests to APNs and Sending push notifications using command-line tools.

## See Also

### Location updates

Getting the current location of a device

Start location services and provide information the system needs to optimize power usage for those services.

Handling location updates in the background

Configure your app to receive location updates when it isn’t running in the foreground.

class CLLocation

The latitude, longitude, and course information reported by the system.

struct CLLocationCoordinate2D

The latitude and longitude associated with a location, specified using the WGS 84 reference frame.

class CLFloor

The floor of a building on which the user’s device is located.

class CLVisit

Information about the user’s location during a specific period of time.

class CLLocationSourceInformation

Information about the source that provides a location.

Monitoring location changes with Core Location

Define boundaries and act on user location updates.

class CLServiceSession

