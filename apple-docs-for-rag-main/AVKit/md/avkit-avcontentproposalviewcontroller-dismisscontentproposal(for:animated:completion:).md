

- AVKit
- AVContentProposalViewController
-  dismissContentProposal(for:animated:completion:) 

Instance Method

# dismissContentProposal(for:animated:completion:)

Dismisses the current content proposal.

tvOS 10.0+

``` source
@MainActor
func dismissContentProposal(
    for action: AVContentProposalAction,
    animated: Bool,
    completion block: (() -> Void)? = nil
)
```

``` source
@MainActor
func dismissContentProposal(
    for action: AVContentProposalAction,
    animated: Bool
) async
```

## Parameters 

`action`  

A content proposal action that indicates whether the user accepted, rejected, or deferred the content proposal.

`animated`  

A Boolean value that indicates whether the content proposal dismisses in an animated manner.

`block`  

An optional callback that the system calls when its hidden the conten proposal.

## Mentioned in 

Presenting Content Proposals in tvOS

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func dismissContentProposal(for action: AVContentProposalAction, animated: Bool) async
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method to indicate the user action when leaving this proposal.

## See Also

### Dismissing the Proposal

enum AVContentProposalAction

Constant that indicate the action a user takes when dismissing a content proposal.

