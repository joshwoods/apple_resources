

- AppKit
- NSScrubberDelegate
-  didFinishInteracting(with:) 

Instance Method

# didFinishInteracting(with:)

Tells the delegate that a pan or scroll interaction with the scrubber has ended.

macOS 10.12.2+

``` source
@MainActor
optional func didFinishInteracting(with scrubber: NSScrubber)
```

## Parameters 

`scrubber`  

The scrubber the user was interacting with.

## See Also

### Tracking user interaction

func didBeginInteracting(with: NSScrubber)

Tells the delegate that the user is panning or scrolling the scrubber.

func didCancelInteracting(with: NSScrubber)

Tells the delegate that a user interaction with the scrubber has been canceled.

