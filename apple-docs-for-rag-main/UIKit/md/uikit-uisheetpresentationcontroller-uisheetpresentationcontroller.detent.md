

- UIKit
- UISheetPresentationController
-  UISheetPresentationController.Detent 

Class

# UISheetPresentationController.Detent

An object that represents a height where a sheet naturally rests.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
class Detent
```

## Topics

### Creating a system detent

class func large() -> Self

Creates a system detent for a sheet at full height.

class func medium() -> Self

Creates a system detent for a sheet that’s approximately half the height of the screen, and is inactive in compact height.

### Creating a custom detent

static func custom(identifier: UISheetPresentationController.Detent.Identifier?, resolver: (any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?) -> UISheetPresentationController.Detent

Creates a custom detent for a sheet by computing its value according to the properties of the provided context.

func resolvedValue(in: any UISheetPresentationControllerDetentResolutionContext) -> CGFloat?

Resolves a detent to its value.

protocol UISheetPresentationControllerDetentResolutionContext

A context for resolving custom detent values.

### Identifying a detent

var identifier: UISheetPresentationController.Detent.Identifier

The identifier of the detent.

struct Identifier

Constants that identify system detent sizes.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Specifying the height

var detents: [UISheetPresentationController.Detent]

The array of heights where a sheet can rest.

var selectedDetentIdentifier: UISheetPresentationController.Detent.Identifier?

The identifier of the most recently selected detent.

