

- Bundle Resources
- Information Property List
-  NSLocationAlwaysAndWhenInUseUsageDescription 

Property List Key

# NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

## Details 

Name  
Privacy - Location Always and When In Use Usage Description

Type  

string

## Discussion

Use this key if your iOS app accesses location information while running in the background. If your app only needs location information when in the foreground, use NSLocationWhenInUseUsageDescription instead. For more information, see Choosing the Location Services Authorization to Request.

If you need location information in a macOS app, use NSLocationUsageDescription instead. If your iOS app deploys to versions earlier than iOS 11, see NSLocationAlwaysUsageDescription.

Important

This key is required if your iOS app uses APIs that access the user’s location information at all times.

## See Also

### Location

Choosing the Location Services Authorization to Request

Determine the authorization your app needs to access location data.

NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

**Name:** Privacy - Location Usage Description

NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

**Name:** Privacy - Location When In Use Usage Description

NSLocationTemporaryUsageDescriptionDictionary

A collection of messages that explain why the app is requesting temporary access to the user’s location.

**Name:** Privacy - Location Temporary Usage Description Dictionary

NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

**Name:** Privacy - Location Always Usage Description

Deprecated

NSWidgetWantsLocation

A Boolean value that indicates a widget uses the user’s location information.

**Name:** Widget wants location

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

**Name:** Privacy - Location Default Accuracy Reduced

