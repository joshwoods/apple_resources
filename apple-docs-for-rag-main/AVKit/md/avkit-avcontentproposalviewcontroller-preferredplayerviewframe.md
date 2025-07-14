

- AVKit
- AVContentProposalViewController
-  preferredPlayerViewFrame 

Instance Property

# preferredPlayerViewFrame

The preferred presentation frame of the player view while the content proposal is active.

tvOS 10.0+

``` source
@MainActor
var preferredPlayerViewFrame: CGRect { get }
```

## Mentioned in 

Presenting Content Proposals in tvOS

## Discussion

This value defaults to a rectangle that represents the entire screen bounds, but custom view controllers may return a smaller rectangle, or zero to hide the player view completely. If you return a rectangle smaller that the full-screen bounds, the player view animates its frame to its new size and position.

## See Also

### Configuring the Proposal

var contentProposal: AVContentProposal?

A prosal of content to play.

class AVContentProposal

An object that describes the content to propose playing after the current item finishes.

var dateOfAutomaticAcceptance: Date?

The date that the system automatically accepts a proposal if the user doesn’t intervene.

var playerLayoutGuide: UILayoutGuide

A layout guide that tracks the size and location of the player view.

