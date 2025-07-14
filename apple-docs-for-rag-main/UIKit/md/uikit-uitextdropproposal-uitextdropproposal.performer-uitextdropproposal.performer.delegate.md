

- UIKit
- UITextDropProposal
- UITextDropProposal.Performer
-  UITextDropProposal.Performer.delegate 

Case

# UITextDropProposal.Performer.delegate

A performer type that indicates the delegate object is responsible for doing the drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case delegate
```

## Discussion

If this performer is used, the delegate must implement the textDroppableView(_:willPerformDrop:) method. Otherwise, the text view handles the drop operation, which is the same behavior as specifying UITextDropProposal.Performer.view as the performer.

## See Also

### Performers

case view

A performer type that indicates that the text view is responsible for doing the drop operation.

