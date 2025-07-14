

- UIKit
- UIPickerView
-  reloadAllComponents() 

Instance Method

# reloadAllComponents()

Reloads all components of the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func reloadAllComponents()
```

## Discussion

Calling this method causes the picker view to query the delegate for new data for all components.

## See Also

### Reloading the picker view

func reloadComponent(Int)

Reloads a particular component of the picker view.

