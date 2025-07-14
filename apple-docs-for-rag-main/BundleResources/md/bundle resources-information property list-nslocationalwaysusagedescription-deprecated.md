

- Bundle Resources
- Information Property List
-  NSLocationAlwaysUsageDescription Deprecated

Property List Key

# NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0Deprecated

Deprecated

For apps deployed to targets in iOS 11 and later, use NSLocationAlwaysAndWhenInUseUsageDescription instead.

## Details 

Name  
Privacy - Location Always Usage Description

Type  

string

## Discussion

Use this key if your iOS app accesses location information in the background, and you deploy to a target earlier than iOS 11. In that case, add both this key and NSLocationAlwaysAndWhenInUseUsageDescription to your app’s `Info.plist` file with the same message. Apps running on older versions of the OS use the message associated with NSLocationAlwaysUsageDescription, while apps running on later versions use the one associated with NSLocationAlwaysAndWhenInUseUsageDescription.

If your app only needs location information when in the foreground, use NSLocationWhenInUseUsageDescription instead. For more information, see Choosing the Location Services Authorization to Request.

If you need location information in a macOS app, use NSLocationUsageDescription instead.

Important

This key is required if your iOS app uses APIs that access the user’s location at all times and deploys to targets earlier than iOS 11.

## See Also

### Location

Choosing the Location Services Authorization to Request

Determine the authorization your app needs to access location data.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

**Name:** Privacy - Location Always and When In Use Usage Description

NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

**Name:** Privacy - Location Usage Description

NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

**Name:** Privacy - Location When In Use Usage Description

NSLocationTemporaryUsageDescriptionDictionary

A collection of messages that explain why the app is requesting temporary access to the user’s location.

**Name:** Privacy - Location Temporary Usage Description Dictionary

NSWidgetWantsLocation

A Boolean value that indicates a widget uses the user’s location information.

**Name:** Widget wants location

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

**Name:** Privacy - Location Default Accuracy Reduced

