

- AppKit
-  NSScrubberDelegate 

Protocol

# NSScrubberDelegate

A set of methods that a scrubber delegate implements to respond to user interactions.

macOS

``` source
protocol NSScrubberDelegate : NSObjectProtocol
```

## Topics

### Handling item selection and highlighting

func scrubber(NSScrubber, didSelectItemAt: Int)

Tells the delegate that the item at the specified index was selected.

func scrubber(NSScrubber, didHighlightItemAt: Int)

Tells the delegate that the item at the specified index was highlighted.

### Handling scrubber scrolling

func scrubber(NSScrubber, didChangeVisibleRange: NSRange)

Tells the delegate that the range of items currently visible in the scrubber has changed.

### Tracking user interaction

func didBeginInteracting(with: NSScrubber)

Tells the delegate that the user is panning or scrolling the scrubber.

func didFinishInteracting(with: NSScrubber)

Tells the delegate that a pan or scroll interaction with the scrubber has ended.

func didCancelInteracting(with: NSScrubber)

Tells the delegate that a user interaction with the scrubber has been canceled.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSScrubberFlowLayoutDelegate

## See Also

### Scrubbers

class NSScrubber

A customizable item picker control for the Touch Bar.

protocol NSScrubberDataSource

A set of methods that a scrubber data source object implements to provide items to the scrubber from an associated data collection in your app.

