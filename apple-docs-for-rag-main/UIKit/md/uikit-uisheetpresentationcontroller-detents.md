

- UIKit
- UISheetPresentationController
-  detents 

Instance Property

# detents

The array of heights where a sheet can rest.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
var detents: [UISheetPresentationController.Detent] { get set }
```

## Discussion

The default value is an array that contains the value large(). This array must contain at least one element. When you set this value, specify detents in order from smallest to largest height.

## See Also

### Specifying the height

var selectedDetentIdentifier: UISheetPresentationController.Detent.Identifier?

The identifier of the most recently selected detent.

class Detent

An object that represents a height where a sheet naturally rests.

