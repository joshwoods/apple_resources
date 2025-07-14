

- StoreKit
- SKAdNetwork
-  startImpression(\_:completionHandler:) 

Type Method

# startImpression(\_:completionHandler:)

Indicates that your app is presenting a view-through ad to the user.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+

``` source
class func startImpression(
    _ impression: SKAdImpression,
    completionHandler completion: (((any Error)?) -> Void)? = nil
)
```

``` source
class func startImpression(_ impression: SKAdImpression) async throws
```

## Parameters 

`impression`  

An instance of SKAdImpression with the properties set for the view-through ad that you’re presenting.

`completion`  

The callback handler you provide to handle any tasks relevant to the start of the ad impression.

## Mentioned in 

Generating the signature to validate view-through ads

SKAdNetwork 2.2 release notes

Signing and providing ads

## Discussion

Call this method when you start presenting the view-through ad to the user. If you call startImpression(_:completionHandler:) more than once for the same advertised app before calling endImpression(_:completionHandler:), the latest impression overwrites the earlier impression.

Call endImpression(_:completionHandler:) when the impression ends and is no longer visible to the user.

Note

To ensure that SKAdNetwork records the impression, call endImpression(_:completionHandler:) after the impression ends, regardless of whether startImpression(_:completionHandler:) returns an error in the completion handler.

## See Also

### Signing view-through ads

Generating the signature to validate view-through ads

Initiate install validation by displaying a view-through ad with signed parameters.

class SKAdImpression

A class that defines an ad impression for a view-through ad.

class func endImpression(SKAdImpression, completionHandler: (((any Error)?) -> Void)?)

Indicates that your app is no longer presenting a view-through ad to the user.

