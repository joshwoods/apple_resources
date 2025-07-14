

- UIKit
- UIAppearance
-  appearance(for:) 

Type Method

# appearance(for:)

Returns the appearance proxy for the receiver that has the passed trait collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
static func appearance(for trait: UITraitCollection) -> Self
```

**Required**

## Parameters 

`trait`  

The trait collection used for matching.

## Return Value

The appearance proxy for the receiver.

## See Also

### Working with the appearance proxy

static func appearance() -> Self

Returns the appearance proxy for the receiver.

**Required**

static func appearance(whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe.

**Required**

static func appearance(for: UITraitCollection, whenContainedInInstancesOf: [any UIAppearanceContainer.Type]) -> Self

Returns the appearance proxy for the object when it’s contained in the hierarchy the specified classes describe and has the specified trait collection.

**Required**

