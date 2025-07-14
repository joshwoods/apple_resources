

- AVKit
- AVContentProposal
-  contentTimeForTransition 

Instance Property

# contentTimeForTransition

The time within the timeline of the current player item when the content proposal presentation should begin.

tvOS 10.0+

``` source
var contentTimeForTransition: CMTime { get }
```

## Discussion

The time value commonly marks the beginning of the end credits in a television show or movie. For other content, this may be at the very end of the video. The default value, indefinite, indicates that the transition should occur at the very end of the current player item’s end time; this is equivalent to using the duration of the asset.

## See Also

### Configuring the Content Proposal

var title: String

The title of the proposed content.

var previewImage: UIImage?

The preview image of the proposed item.

var metadata: [AVMetadataItem]

Optional custom metadata associated with the proposed item.

var automaticAcceptanceInterval: TimeInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

var url: URL?

The URL of the proposed content.

