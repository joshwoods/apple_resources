

- UIKit
- UIAppearance
-  appearance() 

Type Method

# appearance()

Returns the appearance proxy for the receiver.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
static func appearance() -> Self
```

**Required**

## Return Value

The appearance proxy for the receiver.

## See Also

### Working with the appearance proxy

static func appearance(for: UITraitCollection) -> Self

Returns the appearance proxy for the receiver that has the passed trait collection.

**Required**

static func appearance(whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe.

**Required**

static func appearance(for: UITraitCollection, whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe and has the specified trait collection.

**Required**

