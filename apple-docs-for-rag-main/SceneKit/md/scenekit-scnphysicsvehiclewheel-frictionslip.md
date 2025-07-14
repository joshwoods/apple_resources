

- SceneKit
- SCNPhysicsVehicleWheel
-  frictionSlip 

Instance Property

# frictionSlip

The traction between the wheel and any surface in contact with it.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var frictionSlip: CGFloat { get set }
```

## Discussion

The default value of this property is `1.0`. Lower values result in better traction, and higher values make the wheel more likely to slip (causing it to spin freely instead of moving the vehicle).

