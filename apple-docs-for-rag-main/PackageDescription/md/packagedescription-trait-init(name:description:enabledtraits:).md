

- PackageDescription
- Trait
-  init(name:description:enabledTraits:) 

Initializer

# init(name:description:enabledTraits:)

Initializes a new trait.

SwiftPM 6.1+

``` source
init(
    name: String,
    description: String? = nil,
    enabledTraits: Set = []
)
```

## Parameters 

`name`  

The trait’s canonical name.

`description`  

The trait’s description.

`enabledTraits`  

A set of other traits of this package that this trait enables.

