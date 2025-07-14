

- AVKit
- AVContentProposalViewController
-  playerLayoutGuide 

Instance Property

# playerLayoutGuide

A layout guide that tracks the size and location of the player view.

tvOS 10.0+

``` source
@MainActor
var playerLayoutGuide: UILayoutGuide { get }
```

## Mentioned in 

Presenting Content Proposals in tvOS

## Discussion

The view controller can constrain its views using the anchors of the player layout guide, which has the same size and position as the player view. The layout guide is always relative to the current preferredPlayerViewFrame property value.

## See Also

### Configuring the Proposal

var contentProposal: AVContentProposal?

A prosal of content to play.

class AVContentProposal

An object that describes the content to propose playing after the current item finishes.

var dateOfAutomaticAcceptance: Date?

The date that the system automatically accepts a proposal if the user doesn’t intervene.

var preferredPlayerViewFrame: CGRect

The preferred presentation frame of the player view while the content proposal is active.

