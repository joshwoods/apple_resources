

- UIKit
- UIAttachmentBehavior
-  init(item:offsetFromCenter:attachedTo:offsetFromCenter:) 

Initializer

# init(item:offsetFromCenter:attachedTo:offsetFromCenter:)

Initializes an attachment behavior that connects a specified point in one dynamic item to a specified point in another dynamic item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
init(
    item item1: any UIDynamicItem,
    offsetFromCenter offset1: UIOffset,
    attachedTo item2: any UIDynamicItem,
    offsetFromCenter offset2: UIOffset
)
```

## Parameters 

`item1`  

The first of two dynamic items connected by the attachment behavior.

`offset1`  

The offset from the center of `item1` at which to create the attachment. Specifying zero creates the attachment at the center of `item1`.

`item2`  

The second of two dynamic items connected by the attachment behavior.

`offset2`  

The offset from the center of `item2` at which to create the attachment. Specifying zero creates the attachment at the center of `item2`.

## Return Value

The initialized attachment behavior, or `nil` if there was a problem initializing the object.

## Discussion

The behavior created by this method acts like a solid rod connecting the two items at the specified offsets from their center points. Forces applied to one item push or pull the other item accordingly. The items are free to rotate around each other but always remain the same distance apart.

The attachment object returned by this method is of type UIAttachmentBehavior.AttachmentType.items.

## See Also

### Creating and initializing attachment behavior objects

class func slidingAttachment(with: any UIDynamicItem, attachmentAnchor: CGPoint, axisOfTranslation: CGVector) -> Self

Creates and returns an attachment behavior where one item slides along the specified axis.

class func slidingAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint, axisOfTranslation: CGVector) -> Self

Creates and returns an attachment behavior where two items are fixed to points that slide along the specified axis.

class func fixedAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint) -> Self

Creates and returns an attachment behavior where the two items are fixed together through the specified anchor point.

class func limitAttachment(with: any UIDynamicItem, offsetFromCenter: UIOffset, attachedTo: any UIDynamicItem, offsetFromCenter: UIOffset) -> Self

Creates and returns an attachment behavior object where two items are constrained by a maximum distance from one another.

class func pinAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint) -> Self

Creates and returns an attachment behavior where the two items are pinned to, and move around, an anchor point

convenience init(item: any UIDynamicItem, attachedToAnchor: CGPoint)

Initializes a behavior where the center of a dynamic item is attached to the specified anchor point.

convenience init(item: any UIDynamicItem, attachedTo: any UIDynamicItem)

Initializes a behavior where the centers of two dynamic items are attached to each other.

init(item: any UIDynamicItem, offsetFromCenter: UIOffset, attachedToAnchor: CGPoint)

Initializes a behavior where the specified point in a dynamic item is attached to an anchor point.

