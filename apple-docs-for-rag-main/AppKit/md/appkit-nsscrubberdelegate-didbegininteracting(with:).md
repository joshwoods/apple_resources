

- AppKit
- NSScrubberDelegate
-  didBeginInteracting(with:) 

Instance Method

# didBeginInteracting(with:)

Tells the delegate that the user is panning or scrolling the scrubber.

macOS 10.12.2+

``` source
@MainActor
optional func didBeginInteracting(with scrubber: NSScrubber)
```

## Parameters 

`scrubber`  

The scrubber the user is interacting with.

## See Also

### Tracking user interaction

func didFinishInteracting(with: NSScrubber)

Tells the delegate that a pan or scroll interaction with the scrubber has ended.

func didCancelInteracting(with: NSScrubber)

Tells the delegate that a user interaction with the scrubber has been canceled.

