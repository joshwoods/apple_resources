

- UIKit
- UITextDropProposal
- UITextDropProposal.Performer
-  UITextDropProposal.Performer.view 

Case

# UITextDropProposal.Performer.view

A performer type that indicates that the text view is responsible for doing the drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case view
```

## Discussion

This performer is the default for a UITextDropProposal object. If this performer is used, the textDroppableView(_:willPerformDrop:) method is called (if implemented). However, implementing the delegate method isn’t required when using this performer.

## See Also

### Performers

case delegate

A performer type that indicates the delegate object is responsible for doing the drop operation.

