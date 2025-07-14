

- SceneKit
- SCNParticleSystem
-  init(named:inDirectory:) 

Initializer

# init(named:inDirectory:)

Loads a particle system from a file in the app’s bundle resources.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
convenience init?(
    named name: String,
    inDirectory directory: String?
)
```

## Parameters 

`name`  

The name of a particle system file in the app’s bundle resources directory, with or without the `.scnp` extension.

`directory`  

The subdirectory path in the app’s bundle resources directory.

## Return Value

A new particle system instantiated from the contents of the file.

## Discussion

A SceneKit particle file created by Xcode contains an archived SCNParticleSystem instance, so you can also use the NSKeyedArchiver and NSKeyedUnarchiver classes to write and read particle files.

