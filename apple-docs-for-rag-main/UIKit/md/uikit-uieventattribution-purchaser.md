

- UIKit
- UIEventAttribution
-  purchaser 

Instance Property

# purchaser

The entity that purchased the ad or content.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var purchaser: String { get }
```

## Discussion

This property contains the name of the party that purchased the ad or other content. For example, for an in-app ad, this would contain the name of the company or individual that purchased the advertisement. The system may truncate this field if it’s longer than 100 characters.

## See Also

### Setting attribution details

var destinationURL: URL

The destination URL to attribute.

var reportEndpoint: URL?

The URL that receives attribution data.

var sourceDescription: String

A string describing the source tapped to launch the external link.

var sourceIdentifier: UInt8

A number that identifies the source of the attribution.

