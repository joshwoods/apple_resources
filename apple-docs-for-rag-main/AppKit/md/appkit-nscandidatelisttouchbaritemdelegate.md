

- AppKit
-  NSCandidateListTouchBarItemDelegate 

Protocol

# NSCandidateListTouchBarItemDelegate

A set of methods that a candidate list item delegate uses to enable selection state and list visibility.

macOS

``` source
protocol NSCandidateListTouchBarItemDelegate : NSObjectProtocol
```

## Topics

### Handling selection changes

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, beginSelectingCandidateAt: Int)

Tells the delegate that the user has started touching one of the candidates in the candidate list item.

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, changeSelectionFromCandidateAt: Int, to: Int)

Tells the delegate that user has moved from touching one candidate in the candidate list item to another.

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, endSelectingCandidateAt: Int)

Tells the delegate that a user has stopped touching candidates in the candidate list item.

### Handling visibility changes

func candidateListTouchBarItem(NSCandidateListTouchBarItem&lt;AnyObject>, changedCandidateListVisibility: Bool)

Tells the delegate that the visibility of the candidate list has changed.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTextView

## See Also

### Providing a client and a delegate

var client: (any NSView &amp; NSTextInputClient)?

The client object for the candidate list item.

var delegate: (any NSCandidateListTouchBarItemDelegate)?

The delegate of the candidate list item.

