

- SceneKit
- SCNShadable
-  program 

Instance Property

# program

A program used when rendering the object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
optional var program: SCNProgram? { get set }
```

## Discussion

Assigning a program to an object overrides all other rendering parameters, including material settings and shader modifiers.

