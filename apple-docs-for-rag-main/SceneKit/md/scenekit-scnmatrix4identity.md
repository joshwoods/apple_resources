

- SceneKit
-  SCNMatrix4Identity 

Global Variable

# SCNMatrix4Identity

The 4 x 4 identity matrix.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

**macOS**

``` source
let SCNMatrix4Identity: SCNMatrix4
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
let SCNMatrix4Identity: SCNMatrix4
```

## Discussion

Elements on the diagonal of this matrix are `1.0`; all other elements are `0.0`. Multiplying another matrix by the identity matrix or multiplying the identity matrix by another matrix yields the other matrix.

