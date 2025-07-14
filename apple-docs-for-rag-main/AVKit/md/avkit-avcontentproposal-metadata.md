

- AVKit
- AVContentProposal
-  metadata 

Instance Property

# metadata

Optional custom metadata associated with the proposed item.

tvOS 10.0+

``` source
var metadata: [AVMetadataItem] { get set }
```

## Discussion

In addition to the title and preview image, you can associate any custom metadata you need for the presentation of this content proposal.

## See Also

### Configuring the Content Proposal

var contentTimeForTransition: CMTime

The time within the timeline of the current player item when the content proposal presentation should begin.

var title: String

The title of the proposed content.

var previewImage: UIImage?

The preview image of the proposed item.

var automaticAcceptanceInterval: TimeInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

var url: URL?

The URL of the proposed content.

