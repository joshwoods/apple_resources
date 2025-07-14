

- UIKit
- UISheetPresentationControllerDetentResolutionContext
-  containerTraitCollection 

Instance Property

# containerTraitCollection

The trait collection of the sheet’s container view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
@MainActor
var containerTraitCollection: UITraitCollection { get }
```

**Required**

## Discussion

The value of this property is the same as the window’s traitCollection, and doesn’t include overrides from the sheet’s overrideTraitCollection.

## See Also

### Accessing the properties of the context

var maximumDetentValue: CGFloat

The maximum value of a detent.

**Required**

