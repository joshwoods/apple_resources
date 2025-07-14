

- AVKit
- AVContentProposalViewController
-  playerViewController 

Instance Property

# playerViewController

The player view controller that presents a content proposal.

tvOS 10.0+

``` source
@MainActor
weak var playerViewController: AVPlayerViewController? { get }
```

## Discussion

The framework sets this property value during the presentation of the content proposal. It may be `nil` at other times.

