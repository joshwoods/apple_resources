

- Link Presentation
- LPLinkView
-  metadata 

Instance Property

# metadata

The metadata from which to generate a rich presentation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var metadata: LPLinkMetadata { get set }
```

## Discussion

This can either be generated automatically from a URL by LPMetadataProvider, or manually constructed with the desired data.

