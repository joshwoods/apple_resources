

- AVKit
- AVContentProposalViewController
-  contentProposal 

Instance Property

# contentProposal

A prosal of content to play.

tvOS 10.0+

``` source
@MainActor
var contentProposal: AVContentProposal? { get }
```

## Discussion

The associated player view controller sets this property value.

## See Also

### Configuring the Proposal

class AVContentProposal

An object that describes the content to propose playing after the current item finishes.

var dateOfAutomaticAcceptance: Date?

The date that the system automatically accepts a proposal if the user doesn’t intervene.

var playerLayoutGuide: UILayoutGuide

A layout guide that tracks the size and location of the player view.

var preferredPlayerViewFrame: CGRect

The preferred presentation frame of the player view while the content proposal is active.

