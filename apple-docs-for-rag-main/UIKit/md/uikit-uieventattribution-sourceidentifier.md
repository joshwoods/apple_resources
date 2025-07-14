

- UIKit
- UIEventAttribution
-  sourceIdentifier 

Instance Property

# sourceIdentifier

A number that identifies the source of the attribution.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var sourceIdentifier: UInt8 { get }
```

## Discussion

This property contains an integer, between 0 and 255, that identifies the source of the attribution. For example, for an ad, `sourceIdentifier` might contain a campaign identifier so the advertiser can measure the effectiveness of different advertising campaigns.

This field corresponds to the `source_id` field of a web attribution.

## See Also

### Setting attribution details

var destinationURL: URL

The destination URL to attribute.

var purchaser: String

The entity that purchased the ad or content.

var reportEndpoint: URL?

The URL that receives attribution data.

var sourceDescription: String

A string describing the source tapped to launch the external link.

