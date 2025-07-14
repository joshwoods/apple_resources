

- StoreKit
- SKAdNetwork
-  endImpression(\_:completionHandler:) 

Type Method

# endImpression(\_:completionHandler:)

Indicates that your app is no longer presenting a view-through ad to the user.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
class func endImpression(
    _ impression: SKAdImpression,
    completionHandler completion: (((any Error)?) -> Void)? = nil
)
```

``` source
class func endImpression(_ impression: SKAdImpression) async throws
```

## Parameters 

`impression`  

An instance of SKAdImpression with the properties set for the view-through ad that you presented. This must be the same instance you provide in startImpression(_:completionHandler:).

`completion`  

The callback handler you provide to handle any tasks relevant to concluding the ad impression.

## Mentioned in 

Generating the signature to validate view-through ads

Signing and providing ads

SKAdNetwork 2.2 release notes

## Discussion

Call this method when you end the presentation of a view-through ad and it’s no longer visible to the user. To help ensure it’s a valid impression, StoreKit only records the impression if the ad displays for a minimum amount of time. That minimum is 2 seconds on devices running iOS 15.4 and iPadOS 15.4 and later, and 3 seconds on devices running earlier versions of iOS and iPadOS. If the app displays the ad for fewer than the minimum number of seconds, StoreKit doesn’t record the ad impression for attribution.

Note

To ensure that SKAdNetwork records the impression, call endImpression(_:completionHandler:) after the impression ends, regardless of whether startImpression(_:completionHandler:) returns an error in the completion handler.

StoreKit records a maximum of 15 view-through ad impressions per source app for various products before discarding the oldest-recorded impression.

For more information about ad impressions and attributions, see Receiving ad attributions and postbacks.

## See Also

### Signing view-through ads

Generating the signature to validate view-through ads

Initiate install validation by displaying a view-through ad with signed parameters.

class SKAdImpression

A class that defines an ad impression for a view-through ad.

class func startImpression(SKAdImpression, completionHandler: (((any Error)?) -> Void)?)

Indicates that your app is presenting a view-through ad to the user.

