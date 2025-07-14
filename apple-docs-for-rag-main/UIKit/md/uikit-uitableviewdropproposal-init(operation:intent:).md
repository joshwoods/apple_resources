

- UIKit
- UITableViewDropProposal
-  init(operation:intent:) 

Initializer

# init(operation:intent:)

Creates a drop proposal object that specifies how to incorporate the dropped content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(
    operation: UIDropOperation,
    intent: UITableViewDropProposal.Intent
)
```

## Parameters 

`operation`  

The type of operation that you want to perform. Use this parameter to specify whether you want to move the original item to this new location, move a copy of the content, or prevent the content from being inserted at this location. For a list of possible values, see UIDropOperation.

`intent`  

The option for how to incorporate the content into the table view. You can insert the content between items or add it to an existing item.

## Return Value

An initialized drop proposal.

