

- AVKit
- AVContentProposal
-  url 

Instance Property

# url

The URL of the proposed content.

tvOS 10.0+

``` source
var url: URL? { get set }
```

## Discussion

Use this property value to initialize a new AVPlayerItem to play when the user accepts the content proposal. If the value of this property is `nil`, the AVPlayerViewControllerDelegate must handle the content proposal acceptance.

## See Also

### Configuring the Content Proposal

var contentTimeForTransition: CMTime

The time within the timeline of the current player item when the content proposal presentation should begin.

var title: String

The title of the proposed content.

var previewImage: UIImage?

The preview image of the proposed item.

var metadata: [AVMetadataItem]

Optional custom metadata associated with the proposed item.

var automaticAcceptanceInterval: TimeInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

