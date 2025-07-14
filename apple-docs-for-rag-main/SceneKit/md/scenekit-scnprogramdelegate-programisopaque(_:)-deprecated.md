

- SceneKit
- SCNProgramDelegate
-  programIsOpaque(\_:) Deprecated

Instance Method

# programIsOpaque(\_:)

Asks the delegate whether fragments rendered by a program are opaque.

macOS 10.8–10.10Deprecated

``` source
optional func programIsOpaque(_ program: SCNProgram) -> Bool
```

Deprecated

Use the isOpaque property of the SCNProgram object instead.

## Parameters 

`program`  

The queried program.

## Return Value

true if all fragments rendered by the program are opaque; false if the program renders fragments whose alpha value is less than `1.0`.

