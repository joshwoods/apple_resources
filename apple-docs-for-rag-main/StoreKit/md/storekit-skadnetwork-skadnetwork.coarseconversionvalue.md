

- StoreKit
- SKAdNetwork
-  SKAdNetwork.CoarseConversionValue 

Structure

# SKAdNetwork.CoarseConversionValue

Coarse values to use for updating conversion values.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+

``` source
struct CoarseConversionValue
```

## Mentioned in 

SKAdNetwork 4 release notes

## Discussion

When you provide the coarse conversion value to the updatePostbackConversionValue(_:coarseValue:completionHandler:) or updatePostbackConversionValue(_:coarseValue:lockWindow:completionHandler:) methods, use the static constants low, medium, or high.

These constants have no special meaning. The app or ad network can define their meaning, as is useful for their ad campaigns. The app is responsible for assigning a coarse conversion value, as well as the fine conversion value, when it calls one of the conversion value methods. You can determine how the coarse and fine conversion values relate to the types of conversion events you want to measure.

## Topics

### Providing coarse conversion values

static let high: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a high coarse conversion value.

static let low: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a low coarse conversion value.

static let medium: SKAdNetwork.CoarseConversionValue

A string constant value for indicating a medium coarse conversion value.

init(rawValue: String)

Creates a coarse conversion value from the raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Providing conversion information

class func updatePostbackConversionValue(Int, coarseValue: SKAdNetwork.CoarseConversionValue, lockWindow: Bool, completionHandler: (((any Error)?) -> Void)?)

Updates the fine and coarse conversion values and indicates whether to send the postback before the conversion window ends, and calls a completion handler if the update fails.

class func updatePostbackConversionValue(Int, coarseValue: SKAdNetwork.CoarseConversionValue, completionHandler: (((any Error)?) -> Void)?)

Updates the fine and coarse conversion values, and calls a completion handler if the update fails.

class func updatePostbackConversionValue(Int, completionHandler: (((any Error)?) -> Void)?)

Verifies the first launch of an advertised app and, on subsequent calls, updates the conversion value or calls a completion handler if the update fails.

