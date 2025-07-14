

- Game Controller
- GCPhysicalInputSource
-  direction 

Instance Property

# direction

The directional input, if any, that a physical input source involves.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var direction: GCPhysicalInputSourceDirection { get }
```

**Required**

## Discussion

If this property is `nil`, the physical input source doesn’t involve directional input.

## See Also

### Getting directions

struct GCPhysicalInputSourceDirection

The directions that a physical input source involves.

