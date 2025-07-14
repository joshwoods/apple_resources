

- UIKit
- UIPickerViewDataSource
-  numberOfComponents(in:) 

Instance Method

# numberOfComponents(in:)

Asks the data source for the number of components in the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func numberOfComponents(in pickerView: UIPickerView) -> Int
```

**Required**

## Parameters 

`pickerView`  

The picker view requesting the data.

## Return Value

The number of components (or “columns”) that the picker view should display.

## See Also

### Providing counts for the picker view

func pickerView(UIPickerView, numberOfRowsInComponent: Int) -> Int

Asks the data source for the number of rows for a specified component.

**Required**

