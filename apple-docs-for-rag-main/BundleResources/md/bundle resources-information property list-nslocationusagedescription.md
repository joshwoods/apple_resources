

- Bundle Resources
- Information Property List
-  NSLocationUsageDescription 

Property List Key

# NSLocationUsageDescription

A message that tells the user why the app is requesting access to the user’s location information.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedmacOS 10.14+

## Details 

Name  
Privacy - Location Usage Description

Type  

string

## Discussion

Use this key in a macOS app that accesses the user’s location information. In an iOS app, use NSLocationWhenInUseUsageDescription or NSLocationAlwaysAndWhenInUseUsageDescription instead.

Important

This key is required if your macOS app uses APIs that access the user’s location information.

## See Also

### Location

Choosing the Location Services Authorization to Request

Determine the authorization your app needs to access location data.

NSLocationAlwaysAndWhenInUseUsageDescription

A message that tells the user why the app is requesting access to the user’s location information at all times.

**Name:** Privacy - Location Always and When In Use Usage Description

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

