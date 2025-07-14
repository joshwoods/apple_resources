

- SwiftUI
- ResetFocusAction
-  callAsFunction(in:) 

Instance Method

# callAsFunction(in:)

Asks the focus sytem to reevaluate the default focus item.

macOS 12.0+tvOS 14.0+watchOS 7.0+

``` source
func callAsFunction(in namespace: Namespace.ID)
```

## Parameters 

`namespace`  

The namespace inside which SwiftUI should reevaluate default focus. The namespace should match the focusScope(_:) block where focus requires reevaluation.

## Discussion

The focus system reevaluates default focus when the currently-focused item is within the provided namespace.

