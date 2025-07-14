

- Wallet Passes
-  PersonalizationDictionary 

Object

# PersonalizationDictionary

An object that contains the information you use to personalize a pass.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

``` source
object PersonalizationDictionary
```

## Properties

`personalizationToken`

`string`

 (Required) 

The personalization token for this request. The server must sign and return the token.

`requiredPersonalizationInfo`

PersonalizationDictionary.RequiredPersonalizationInfo

 (Required) 

An object that contains the user-entered information for a personalized pass.

## Topics

### Reading the User Information

object PersonalizationDictionary.RequiredPersonalizationInfo

An object that contains the user-entered information for a personalized pass.

## See Also

### Personalized Passes

Return a Personalized Pass

Create and sign a personalized pass, and send it to a device.

