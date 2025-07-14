

- UIKit
-  UIPickerViewDataSource 

Protocol

# UIPickerViewDataSource

The interface for a picker view’s data source.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
protocol UIPickerViewDataSource : NSObjectProtocol
```

## Overview

The data source of a UIPickerView object must adopt this protocol to mediate between the picker view object and your app’s data model for that picker view. The data source provides the picker view with the number of components, and the number of rows in each component, for displaying the picker view data. Both methods in this protocol are required.

## Topics

### Providing counts for the picker view

func numberOfComponents(in: UIPickerView) -> Int

Asks the data source for the number of components in the picker view.

**Required**

func pickerView(UIPickerView, numberOfRowsInComponent: Int) -> Int

Asks the data source for the number of rows for a specified component.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providing the picker data

var dataSource: (any UIPickerViewDataSource)?

The data source for the picker view.

