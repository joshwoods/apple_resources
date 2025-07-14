

- AVKit
- AVContentProposalViewController
-  dateOfAutomaticAcceptance 

Instance Property

# dateOfAutomaticAcceptance

The date that the system automatically accepts a proposal if the user doesn’t intervene.

tvOS 10.0+

``` source
@MainActor
var dateOfAutomaticAcceptance: Date? { get set }
```

## Discussion

The system schedules the proposal when you present it, and may unschedule it if the user cancels automatic acceptance, manually accepts, or otherwise dismisses the proposal.

Set this property to `nil` to cancel automatic acceptance.

## See Also

### Configuring the Proposal

var contentProposal: AVContentProposal?

A prosal of content to play.

class AVContentProposal

An object that describes the content to propose playing after the current item finishes.

var playerLayoutGuide: UILayoutGuide

A layout guide that tracks the size and location of the player view.

var preferredPlayerViewFrame: CGRect

The preferred presentation frame of the player view while the content proposal is active.

