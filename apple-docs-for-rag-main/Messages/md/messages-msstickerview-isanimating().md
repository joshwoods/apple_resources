

- Messages
- MSStickerView
-  isAnimating() 

Instance Method

# isAnimating()

Returns a Boolean value that indicates whether the sticker is animating.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@MainActor
func isAnimating() -> Bool
```

## Return Value

Returns true if the sticker is animating; otherwise, false.

## See Also

### Controlling Sticker Animation

var animationDuration: TimeInterval

The amount of time it takes to complete the sticker’s animation.

func startAnimating()

Starts the sticker’s animation, beginning with the first frame.

func stopAnimating()

Stops the sticker’s animation.

