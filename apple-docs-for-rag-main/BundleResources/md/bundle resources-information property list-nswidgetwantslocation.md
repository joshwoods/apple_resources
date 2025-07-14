

- Bundle Resources
- Information Property List
-  NSWidgetWantsLocation 

Property List Key

# NSWidgetWantsLocation

A Boolean value that indicates a widget uses the user’s location information.

iOS 14.0+iPadOS 14.0+macOS 11.0+

## Details 

Name  
Widget wants location

Type  

boolean

## Discussion

To access the user’s location information from a widget, set the value to true in the widget extension’s `Info.plist` file.

Before a widget can access location information, the containing app must request authorization from the user. The containing app’s `Info.plist` file must also contain relevant purpose strings. For more information, see Requesting authorization to use location services.

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

NSLocationAlwaysUsageDescription

A message that tells the user why the app is requesting access to the user’s location at all times.

**Name:** Privacy - Location Always Usage Description

Deprecated

NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

**Name:** Privacy - Location Default Accuracy Reduced

