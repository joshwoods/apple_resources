

- AppKit
- NSScrubberDelegate
-  didCancelInteracting(with:) 

Instance Method

# didCancelInteracting(with:)

Tells the delegate that a user interaction with the scrubber has been canceled.

macOS 10.12.2+

``` source
@MainActor
optional func didCancelInteracting(with scrubber: NSScrubber)
```

## Parameters 

`scrubber`  

The scrubber the user is interacting with.

## See Also

### Tracking user interaction

func didBeginInteracting(with: NSScrubber)

Tells the delegate that the user is panning or scrolling the scrubber.

func didFinishInteracting(with: NSScrubber)

Tells the delegate that a pan or scroll interaction with the scrubber has ended.

