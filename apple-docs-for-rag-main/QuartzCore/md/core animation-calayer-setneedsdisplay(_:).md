

- Core Animation
- CALayer
-  setNeedsDisplay(\_:) 

Instance Method

# setNeedsDisplay(\_:)

Marks the region within the specified rectangle as needing to be updated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func setNeedsDisplay(_ r: CGRect)
```

## Parameters 

`r`  

The rectangular region of the layer to mark as invalid. You must specify this rectangle in the layer’s own coordinate system.

## See Also

### Updating Layer Display

func setNeedsDisplay()

Marks the layer’s contents as needing to be updated.

var needsDisplayOnBoundsChange: Bool

A Boolean indicating whether the layer contents must be updated when its bounds rectangle changes.

func displayIfNeeded()

Initiates the update process for a layer if it is currently marked as needing an update.

func needsDisplay() -> Bool

Returns a Boolean indicating whether the layer has been marked as needing an update.

class func needsDisplay(forKey: String) -> Bool

Returns a Boolean indicating whether changes to the specified key require the layer to be redisplayed.

