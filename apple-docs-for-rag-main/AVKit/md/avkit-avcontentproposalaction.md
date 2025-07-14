

- AVKit
-  AVContentProposalAction 

Enumeration

# AVContentProposalAction

Constant that indicate the action a user takes when dismissing a content proposal.

tvOS 9.0+

``` source
enum AVContentProposalAction
```

## Topics

### Actions

case accept

The user accepted the content proposal.

case reject

The user rejected the content proposal.

case `defer`

The user deferred the content proposal.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Dismissing the Proposal

func dismissContentProposal(for: AVContentProposalAction, animated: Bool, completion: (() -> Void)?)

Dismisses the current content proposal.

