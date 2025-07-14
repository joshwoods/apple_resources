

- AVKit
- AVContentProposal
-  previewImage 

Instance Property

# previewImage

The preview image of the proposed item.

tvOS 10.0+

``` source
var previewImage: UIImage? { get }
```

## Discussion

The preview image you provide should typically be a frame from the proposed video, not the poster artwork.

## See Also

### Configuring the Content Proposal

var contentTimeForTransition: CMTime

The time within the timeline of the current player item when the content proposal presentation should begin.

var title: String

The title of the proposed content.

var metadata: [AVMetadataItem]

Optional custom metadata associated with the proposed item.

var automaticAcceptanceInterval: TimeInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

var url: URL?

The URL of the proposed content.

