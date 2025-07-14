

- SceneKit
- SCNTorus
-  init(ringRadius:pipeRadius:) 

Initializer

# init(ringRadius:pipeRadius:)

Creates a torus geometry with the specified ring radius and pipe radius.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    ringRadius: CGFloat,
    pipeRadius: CGFloat
)
```

## Parameters 

`ringRadius`  

The major radius of the torus, defining its circular ring in the x- and z-axis dimensions of its local coordinate space.

`pipeRadius`  

The minor radius of the torus, defining the pipe that encircles the ring.

## Return Value

A new torus geometry.

## Discussion

The torus is centered in its local coordinate system. For example, if you create a torus whose ring radius is `5.0` and pipe radius is `1.0`, it extends from `-6.0` to `6.0` (with a hole through the center from `-4.0` to `4.0`) in the x- and z-axes and from `-1.0` to `1.0` in the y-axis.

