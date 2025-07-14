

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:didAccept:) 

Instance Method

# playerViewController(\_:didAccept:)

Tells the delegate when the user accepts the proposed content.

tvOS 10.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    didAccept proposal: AVContentProposal
)
```

## Parameters 

`playerViewController`  

The player view controller.

`proposal`  

The content proposal.

## Mentioned in 

Presenting Content Proposals in tvOS

## Discussion

Implement this method to replace the player’s current player item with a player item for the proposed content.

## See Also

### Responding to Content Proposals

func playerViewController(AVPlayerViewController, shouldPresent: AVContentProposal) -> Bool

Asks the delegate whether the player view controller presents a content proposal.

func playerViewController(AVPlayerViewController, didReject: AVContentProposal)

Tells the delegate when the user rejects the proposed content.

