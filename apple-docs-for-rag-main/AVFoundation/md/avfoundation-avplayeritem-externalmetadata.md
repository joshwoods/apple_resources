

- AVFoundation
- AVPlayerItem
-  externalMetadata 

Instance Property

# externalMetadata

An array of additional metadata for the player item to supplement or replace an asset’s embedded metadata.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var externalMetadata: [AVMetadataItem] { get set }
```

## Discussion

AVPlayerViewController supports displaying the following metadata identifiers:

- commonKeyTitle

- iTunesMetadataTrackSubTitle

- commonIdentifierArtwork

- commonKeyDescription

- iTunesMetadataKeyContentRating

- quickTimeMetadataKeyGenre

