

- Bundle Resources
- Information Property List
-  NSLocationWhenInUseUsageDescription 

Property List Key

# NSLocationWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information while the app is running in the foreground.

iOS 11.0+iPadOS 11.0+visionOS 1.0+

## Details 

Name  
Privacy - Location When In Use Usage Description

Type  

string

## Discussion

Use this key if your iOS app accesses location information only when running in the foreground. If your app needs location information when in the background, use NSLocationAlwaysAndWhenInUseUsageDescription instead. For more information, see Choosing the Location Services Authorization to Request.

If you need location information in a macOS app, use NSLocationUsageDescription instead.

Important

This key is required if your iOS app uses APIs that access the user’s location information while the app is in use.

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

