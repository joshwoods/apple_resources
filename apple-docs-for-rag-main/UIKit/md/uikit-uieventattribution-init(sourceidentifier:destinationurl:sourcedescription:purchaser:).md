

- UIKit
- UIEventAttribution
-  init(sourceIdentifier:destinationURL:sourceDescription:purchaser:) 

Initializer

# init(sourceIdentifier:destinationURL:sourceDescription:purchaser:)

Initializes a new event attribution object.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
@MainActor
init(
    sourceIdentifier: UInt8,
    destinationURL: URL,
    sourceDescription: String,
    purchaser: String
)
```

## Parameters 

`sourceIdentifier`  

An 8-bit number that identifies the source of the click for attribution. Value must be between `0` and `255`.

`destinationURL`  

The destination URL of the attribution.

`sourceDescription`  

A description of the source of the attribution.

`purchaser`  

A string that describes the entity that purchased the attributed content.

