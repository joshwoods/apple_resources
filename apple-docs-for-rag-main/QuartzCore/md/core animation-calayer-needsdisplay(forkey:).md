

- Core Animation
- CALayer
-  needsDisplay(forKey:) 

Type Method

# needsDisplay(forKey:)

Returns a Boolean indicating whether changes to the specified key require the layer to be redisplayed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
class func needsDisplay(forKey key: String) -> Bool
```

## Parameters 

`key`  

A string that specifies an attribute of the layer.

## Return Value

true if the layer requires a redisplay.

## Discussion

Subclasses can override this method and return true if the layer should be redisplayed when the value of the specified attribute changes. Animations changing the value of the attribute also trigger redisplay.

The default implementation of this method returns false.

## See Also

### Related Documentation

class func defaultAction(forKey: String) -> (any CAAction)?

Returns the default action for the current class.

class func defaultValue(forKey: String) -> Any?

Specifies the default value associated with the specified key.

### Updating Layer Display

func setNeedsDisplay()

Marks the layer’s contents as needing to be updated.

func setNeedsDisplay(CGRect)

Marks the region within the specified rectangle as needing to be updated.

var needsDisplayOnBoundsChange: Bool

A Boolean indicating whether the layer contents must be updated when its bounds rectangle changes.

func displayIfNeeded()

Initiates the update process for a layer if it is currently marked as needing an update.

func needsDisplay() -> Bool

Returns a Boolean indicating whether the layer has been marked as needing an update.

