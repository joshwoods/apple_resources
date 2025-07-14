

- StoreKit
- SKAdNetwork
- SKAdNetwork.CoarseConversionValue
-  init(rawValue:) 

Initializer

# init(rawValue:)

Creates a coarse conversion value from the raw value.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
init(rawValue: String)
```

## Parameters 

`rawValue`  

A string that is one of low, medium, or high.

## Discussion

You don’t need to call the initializer to use coarse conversion values. When you provide the coarse conversion value to the updatePostbackConversionValue(_:coarseValue:completionHandler:) or updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:) methods, use the static constants, low, medium, or high.

## See Also

### Providing coarse conversion values

static let high: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a high coarse conversion value.

static let low: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a low coarse conversion value.

static let medium: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a medium coarse conversion value.

