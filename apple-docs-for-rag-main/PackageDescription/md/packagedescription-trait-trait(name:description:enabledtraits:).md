

- PackageDescription
- Trait
-  trait(name:description:enabledTraits:) 

Type Method

# trait(name:description:enabledTraits:)

Initializes a new trait.

SwiftPM 6.1+

``` source
static func trait(
    name: String,
    description: String? = nil,
    enabledTraits: Set = []
) -> Trait
```

## Parameters 

`name`  

The trait’s canonical name.

`description`  

The trait’s description.

`enabledTraits`  

A set of other traits of this package that this trait enables.

