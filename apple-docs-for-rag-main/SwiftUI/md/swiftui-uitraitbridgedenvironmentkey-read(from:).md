

- SwiftUI
- UITraitBridgedEnvironmentKey
-  read(from:) 

Type Method

# read(from:)

Reads the trait value from the trait collection, and returns the equivalent environment value.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
static func read(from traitCollection: UITraitCollection) -> Self.Value
```

**Required**

## Parameters 

`traitCollection`  

The trait collection to read from.

## See Also

### Managing the keys

static func write(to: inout any UIMutableTraits, value: Self.Value)

Writes the equivalent trait value for the environment value into the mutable traits.

**Required**

