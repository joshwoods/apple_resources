

- SceneKit
- SCNTechnique
-  init(bySequencingTechniques:) 

Initializer

# init(bySequencingTechniques:)

Creates a new rendering technique that combines a series of techniques.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
init?(bySequencingTechniques techniques: [SCNTechnique])
```

## Parameters 

`techniques`  

An array of SCNTechnique objects.

## Return Value

A new technique object.

## Discussion

The new technique applies the effects of the techniques in the order specified in the `techniques` array. Each output of a technique in the array becomes an input to the next technique in the array.

