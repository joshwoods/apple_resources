

- SceneKit
- SCNBillboardAxis
-  all 

Type Property

# all

Align an affected node such that its orientation always matches that of the view.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var all: SCNBillboardAxis { get }
```

## Discussion

This is the default option for newly created billboard constraints.

## See Also

### Constants

static var X: SCNBillboardAxis

Align an affected node such that its x-axis is always parallel to that of the view, leaving it free to rotate otherwise.

static var Y: SCNBillboardAxis

Align an affected node such that its y-axis is always parallel to that of the view, leaving it free to rotate otherwise.

static var Z: SCNBillboardAxis

Align an affected node such that its z-axis is always perpendicular to the viewing plane, leaving it free to rotate otherwise.

