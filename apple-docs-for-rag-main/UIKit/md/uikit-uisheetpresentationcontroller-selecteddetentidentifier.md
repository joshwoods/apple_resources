

- UIKit
- UISheetPresentationController
-  selectedDetentIdentifier 

Instance Property

# selectedDetentIdentifier

The identifier of the most recently selected detent.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@MainActor
var selectedDetentIdentifier: UISheetPresentationController.Detent.Identifier? { get set }
```

## Discussion

This property represents the most recent detent that the user selects or that you set programmatically. The default value is `nil`, which means the sheet displays at the smallest detent you specify in detents.

## See Also

### Specifying the height

var detents: [UISheetPresentationController.Detent]

The array of heights where a sheet can rest.

class Detent

An object that represents a height where a sheet naturally rests.

