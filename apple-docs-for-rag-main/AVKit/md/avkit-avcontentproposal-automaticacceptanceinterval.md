

- AVKit
- AVContentProposal
-  automaticAcceptanceInterval 

Instance Property

# automaticAcceptanceInterval

The interval between the time playback ends and automatic acceptance of this content proposal.

tvOS 10.0+

``` source
var automaticAcceptanceInterval: TimeInterval { get set }
```

## Discussion

The content proposal displays a countdown timer to reflect this value. Set this value to nan to disable the default, which is automatic acceptance.

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

var url: URL?

The URL of the proposed content.

