

- UIKit
- UIPickerViewDataSource
-  pickerView(\_:numberOfRowsInComponent:) 

Instance Method

# pickerView(\_:numberOfRowsInComponent:)

Asks the data source for the number of rows for a specified component.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func pickerView(
    _ pickerView: UIPickerView,
    numberOfRowsInComponent component: Int
) -> Int
```

**Required**

## Parameters 

`pickerView`  

The picker view requesting the data.

`component`  

A zero-indexed number identifying a component of `pickerView`. Components are numbered left-to-right.

## Return Value

The number of rows for the component.

## See Also

### Providing counts for the picker view

func numberOfComponents(in: UIPickerView) -> Int

Asks the data source for the number of components in the picker view.

**Required**

