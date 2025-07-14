

- UIKit
- UIEventAttribution
-  sourceDescription 

Instance Property

# sourceDescription

A string describing the source tapped to launch the external link.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
var sourceDescription: String { get }
```

## Discussion

This property contains a description of the attribution source. For example, for an ad, `sourceDescription` describes the content of the advertisement that the user tapped.

The system may truncate this field if it’s longer than 100 characters.

## See Also

### Setting attribution details

var destinationURL: URL

The destination URL to attribute.

var purchaser: String

The entity that purchased the ad or content.

var reportEndpoint: URL?

The URL that receives attribution data.

var sourceIdentifier: UInt8

A number that identifies the source of the attribution.

