

- UIKit
- UIPickerView
-  numberOfComponents 

Instance Property

# numberOfComponents

The number of components for the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var numberOfComponents: Int { get }
```

## Discussion

A UIPickerView object fetches the value of this property from the data source and caches it. The default value is `0`.

## See Also

### Getting the dimensions of the picker view

func numberOfRows(inComponent: Int) -> Int

Returns the number of rows for a component.

func rowSize(forComponent: Int) -> CGSize

Returns the size of a row for a component.

