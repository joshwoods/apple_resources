

- Game Controller
- GCDirectionPadElement
-  xyAxes 

Instance Property

# xyAxes

The location of the directional pad represented as a point.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.3+tvOS 17.4+visionOS 1.1+

``` source
var xyAxes: any GCAxis2DInput { get }
```

**Required**

## See Also

### Axes

var xAxis: any GCAxisInput

The input object that represents the x-axis on the directional pad.

**Required**

var yAxis: any GCAxisInput

The input object that represents the y-axis on the directional pad.

**Required**

protocol GCAxis2DInput

The common properties of inputs that provide a normalized point in a two-dimensional coordinate system with a fixed origin.

