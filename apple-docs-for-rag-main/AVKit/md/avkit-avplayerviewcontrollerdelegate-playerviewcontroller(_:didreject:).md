

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:didReject:) 

Instance Method

# playerViewController(\_:didReject:)

Tells the delegate when the user rejects the proposed content.

tvOS 10.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    didReject proposal: AVContentProposal
)
```

## Parameters 

`playerViewController`  

The player view controller.

`proposal`  

The content proposal.

## Mentioned in 

Presenting Content Proposals in tvOS

## See Also

### Responding to Content Proposals

func playerViewController(AVPlayerViewController, shouldPresent: AVContentProposal) -> Bool

Asks the delegate whether the player view controller presents a content proposal.

func playerViewController(AVPlayerViewController, didAccept: AVContentProposal)

Tells the delegate when the user accepts the proposed content.

