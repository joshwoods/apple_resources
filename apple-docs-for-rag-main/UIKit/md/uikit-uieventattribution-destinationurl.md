

- UIKit
- UIEventAttribution
-  destinationURL 

Instance Property

# destinationURL

The destination URL to attribute.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var destinationURL: URL { get }
```

## Discussion

This property contains the URL associated with the event; for example, the `destinationURL` for an advertisement contains the external link opened when the user taps the ad.

This field corresponds to the `attributed_on_site` field of a web attribution.

## See Also

### Setting attribution details

var purchaser: String

The entity that purchased the ad or content.

var reportEndpoint: URL?

The URL that receives attribution data.

var sourceDescription: String

A string describing the source tapped to launch the external link.

var sourceIdentifier: UInt8

A number that identifies the source of the attribution.

