

- UIKit
- UISegmentedControl
-  segmentIndex(identifiedBy:) 

Instance Method

# segmentIndex(identifiedBy:)

The index of a segment with an action that has an identifier matching the identifier you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func segmentIndex(identifiedBy actionIdentifier: UIAction.Identifier) -> Int
```

## Parameters 

`actionIdentifier`  

The UIAction.Identifier to match.

## Return Value

The index of the segment with an action that has a matching identifier, or NSNotFound if no matching action is found.

## See Also

### Managing segments

var numberOfSegments: Int

Returns the number of segments the segmented control has.

func insertSegment(action: UIAction, at: Int, animated: Bool)

Insert a segment with the action you specify at the given index.

func insertSegment(with: UIImage?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it an image as content.

func insertSegment(withTitle: String?, at: Int, animated: Bool)

Inserts a segment at the position you specify and gives it a title as content.

func removeAllSegments()

Removes all segments of the segmented control.

func removeSegment(at: Int, animated: Bool)

Removes the segment you specify from the segmented control, optionally animating the transition.

var selectedSegmentIndex: Int

The index number that identifies the selected segment that the user last touched.

class var noSegment: Int

A segment index value indicating that there’s no selected segment.

