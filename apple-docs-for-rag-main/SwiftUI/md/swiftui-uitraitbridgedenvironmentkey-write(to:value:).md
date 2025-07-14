

- SwiftUI
- UITraitBridgedEnvironmentKey
-  write(to:value:) 

Type Method

# write(to:value:)

Writes the equivalent trait value for the environment value into the mutable traits.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
static func write(
    to mutableTraits: inout any UIMutableTraits,
    value: Self.Value
)
```

**Required**

## Parameters 

`mutableTraits`  

The mutable traits to write to.

`value`  

The environment value to write.

## See Also

### Managing the keys

static func read(from: UITraitCollection) -> Self.Value

Reads the trait value from the trait collection, and returns the equivalent environment value.

**Required**

