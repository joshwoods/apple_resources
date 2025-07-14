

- UIKit
- UIPickerView
-  dataSource 

Instance Property

# dataSource

The data source for the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var dataSource: (any UIPickerViewDataSource)? { get set }
```

## Discussion

The data source must adopt the UIPickerViewDataSource protocol and implement the required methods to return the number of components and the number of rows in each component.

## See Also

### Providing the picker data

protocol UIPickerViewDataSource

The interface for a picker view’s data source.

