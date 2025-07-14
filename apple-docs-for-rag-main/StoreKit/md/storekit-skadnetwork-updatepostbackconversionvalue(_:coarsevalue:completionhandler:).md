

- StoreKit
- SKAdNetwork
-  updatePostbackConversionValue(\_:coarseValue:completionHandler:) 

Type Method

# updatePostbackConversionValue(\_:coarseValue:completionHandler:)

Updates the fine and coarse conversion values, and calls a completion handler if the update fails.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
class func updatePostbackConversionValue(
    _ fineValue: Int,
    coarseValue: SKAdNetwork.CoarseConversionValue,
    completionHandler completion: (((any Error)?) -> Void)? = nil
)
```

``` source
class func updatePostbackConversionValue(
    _ fineValue: Int,
    coarseValue: SKAdNetwork.CoarseConversionValue
) async throws
```

## Parameters 

`fineValue`  

An unsigned 6-bit value `≥0` and `≤63`. The app or the ad network defines the meaning of the conversion value.

`coarseValue`  

An SKAdNetwork.CoarseConversionValue value. The app or the ad network defines the meaning of this value.

`completion`  

An optional completion handler you provide to catch and handle any errors this method encounters when you update a conversion value. Set this value to `nil` if you don’t provide a handler.

## Mentioned in 

SKAdNetwork 4 release notes

Receiving postbacks in multiple conversion windows

Configuring an advertised app

## Discussion

Call this method when the user first launches an app to register the app installation, and optionally again, to update conversion values as the user engages with the app.

This method is identical to calling updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:) with the `lockWindow` parameter set to `false`.

This method returns SKANError.Code.invalidConversionValue if the `fineValue` is outside of the allowed range.

Important

The system ignores calls to this method if the `fineValue` is outside of the valid range. Valid conversion updates your app sends before or after an invalid conversion remain available.

## See Also

### Providing conversion information

class func updatePostbackConversionValue(Int, coarseValue: SKAdNetwork.CoarseConversionValue, lockWindow: Bool, completionHandler: (((any Error)?) -> Void)?)

Updates the fine and coarse conversion values and indicates whether to send the postback before the conversion window ends, and calls a completion handler if the update fails.

struct CoarseConversionValue

Coarse values to use for updating conversion values.

class func updatePostbackConversionValue(Int, completionHandler: (((any Error)?) -> Void)?)

Verifies the first launch of an advertised app and, on subsequent calls, updates the conversion value or calls a completion handler if the update fails.

