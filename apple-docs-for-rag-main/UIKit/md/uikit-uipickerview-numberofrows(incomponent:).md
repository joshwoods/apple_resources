

- UIKit
- UIPickerView
-  numberOfRows(inComponent:) 

Instance Method

# numberOfRows(inComponent:)

Returns the number of rows for a component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func numberOfRows(inComponent component: Int) -> Int
```

## Parameters 

`component`  

A zero-indexed number identifying a component.

## Return Value

The number of rows in the given component.

## Discussion

A picker view fetches the value of this property from the data source and and caches it. The default value is zero.

## See Also

### Getting the dimensions of the picker view

var numberOfComponents: Int

The number of components for the picker view.

func rowSize(forComponent: Int) -> CGSize

Returns the size of a row for a component.

