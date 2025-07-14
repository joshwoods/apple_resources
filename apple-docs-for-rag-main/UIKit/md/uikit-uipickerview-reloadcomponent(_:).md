

- UIKit
- UIPickerView
-  reloadComponent(\_:) 

Instance Method

# reloadComponent(\_:)

Reloads a particular component of the picker view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func reloadComponent(_ component: Int)
```

## Parameters 

`component`  

A zero-indexed number identifying a component of the picker view.

## Discussion

Calling this method causes the picker view to query the delegate for new data for the given component.

## See Also

### Reloading the picker view

func reloadAllComponents()

Reloads all components of the picker view.

