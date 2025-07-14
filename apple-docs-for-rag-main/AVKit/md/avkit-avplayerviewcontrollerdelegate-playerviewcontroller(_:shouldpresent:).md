

- AVKit
- AVPlayerViewControllerDelegate
-  playerViewController(\_:shouldPresent:) 

Instance Method

# playerViewController(\_:shouldPresent:)

Asks the delegate whether the player view controller presents a content proposal.

tvOS 10.0+

``` source
optional func playerViewController(
    _ playerViewController: AVPlayerViewController,
    shouldPresent proposal: AVContentProposal
) -> Bool
```

## Parameters 

`playerViewController`  

The player view controller.

`proposal`  

The content proposal to present.

## Return Value

true if the player view controller should propose the content; otherwise false.

## Mentioned in 

Presenting Content Proposals in tvOS

## See Also

### Responding to Content Proposals

func playerViewController(AVPlayerViewController, didAccept: AVContentProposal)

Tells the delegate when the user accepts the proposed content.

func playerViewController(AVPlayerViewController, didReject: AVContentProposal)

Tells the delegate when the user rejects the proposed content.

