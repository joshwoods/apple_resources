

- Bundle Resources
- Information Property List
-  NSLocationTemporaryUsageDescriptionDictionary 

Property List Key

# NSLocationTemporaryUsageDescriptionDictionary

A collection of messages that explain why the app is requesting temporary access to the user’s location.

iOS 14.0+iPadOS 14.0+macOS 11.0+visionOS 1.0+

## Details 

Name  
Privacy - Location Temporary Usage Description Dictionary

Type  

object

## Discussion

Use this key if your app needs temporary access to full accuracy location information. Provide a dictionary of messages that address different use cases, keyed by strings that you define. For example, if your app suggests nearby coffee shops in one part of the app, and finds nearby friends in another, you could include two entries:

When you request access, select among the messages at run time by providing the associated key to the requestTemporaryFullAccuracyAuthorization(withPurposeKey:) method:

```
// Request location access to find coffee shops.
manager.requestTemporaryFullAccuracyAuthorization(withPurposeKey: "coffee")
```

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

