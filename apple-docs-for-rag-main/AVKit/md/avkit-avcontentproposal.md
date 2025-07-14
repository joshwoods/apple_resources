

- AVKit
-  AVContentProposal 

Class

# AVContentProposal

An object that describes the content to propose playing after the current item finishes.

tvOS 10.0+

``` source
class AVContentProposal
```

## Mentioned in 

Presenting Content Proposals in tvOS

## Overview

A content proposal object models the data about the proposed content such as its title, preview image, presentation time, and content URL. You make a content proposal eligible for presentation by setting it as the nextContentProposal of the current AVPlayerItem.

```
let proposal = AVContentProposal(contentTimeForTransition: time,
                                 title: title,
                                 previewImage: image)
// Set the proposal as the nextContentProposal of the current player item
currentPlayerItem.nextContentProposal = proposal
```

## Topics

### Creating a Content Proposal

init(contentTimeForTransition: CMTime, title: String, previewImage: UIImage?)

Creates a new content proposal with the specified transition time, title, and preview image.

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

var url: URL?

The URL of the proposed content.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuring the Proposal

var contentProposal: AVContentProposal?

A prosal of content to play.

var dateOfAutomaticAcceptance: Date?

The date that the system automatically accepts a proposal if the user doesn’t intervene.

var playerLayoutGuide: UILayoutGuide

A layout guide that tracks the size and location of the player view.

var preferredPlayerViewFrame: CGRect

The preferred presentation frame of the player view while the content proposal is active.

