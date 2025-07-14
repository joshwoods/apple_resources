

- Bundle Resources
- Information Property List
-  NSLocationDefaultAccuracyReduced 

Property List Key

# NSLocationDefaultAccuracyReduced

A Boolean value that indicates whether the app requests reduced location accuracy by default.

iOS 14.0+iPadOS 14.0+visionOS 1.0+watchOS 7.0+

## Details 

Name  
Privacy - Location Default Accuracy Reduced

Type  

boolean

## Attributes 

Default: `NO`

## Discussion

Include this key in your information property list to set your app’s default behavior for location accuracy when it calls the Core Location framework. Set the key value to `true` to prompt the user for reduced accuracy by default; set it to `false` to prompt for full location accuracy. If you don’t include that key in your `Info.plist`, that’s equivalent to setting it to `false`.

Include the key pair in your `Info.plist` file as shown:

```

NSLocationDefaultAccuracyReduced

```

When this key is set to `true`, all Core Location services (location updates, visit monitoring, significant location change, fence monitoring) receive service at the reduced-accuracy service level. Users will see that your app is asking for reduced accuracy because the location authorization prompt will show a map with an approximate location, and your app will have the Precise Location toggled off in Settings \> Privacy \> Location Services . These indicators of an app’s improved privacy are ones that users may value.

If you want to leverage the reduced-accuracy feature to improve privacy in a particular operation without setting this key, use the desiredAccuracy constant kCLLocationAccuracyReduced. This constant causes startUpdatingLocation() to deliver results as if the app were authorized for approximate location until you change the desiredAccuracy constant again.

Setting NSLocationDefaultAccuracyReduced determines the default type of authorization your app gets, but users can override it any time in Settings. Users always control the level of location accuracy they want to share, and can change precision settings in Settings \> Privacy \> Location Services by selecting Precise Location for your app.

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

NSWidgetWantsLocation

A Boolean value that indicates a widget uses the user’s location information.

**Name:** Widget wants location

