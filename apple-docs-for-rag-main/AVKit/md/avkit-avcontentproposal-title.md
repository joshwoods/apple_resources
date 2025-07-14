

- AVKit
- AVContentProposal
-  title 

Instance Property

# title

The title of the proposed content.

tvOS 10.0+

``` source
var title: String { get }
```

## See Also

### Configuring the Content Proposal

var contentTimeForTransition: CMTime

The time within the timeline of the current player item when the content proposal presentation should begin.

var previewImage: UIImage?

The preview image of the proposed item.

var metadata: [AVMetadataItem]

Optional custom metadata associated with the proposed item.

var automaticAcceptanceInterval: TimeInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

var url: URL?

The URL of the proposed content.

