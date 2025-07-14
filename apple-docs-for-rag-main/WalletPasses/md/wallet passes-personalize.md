

- Wallet Passes
-  Personalize 

Object

# Personalize

An object that contains the personalization information for a rewards pass.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

``` source
object Personalize
```

## Properties

`description`

`string`

 (Required) 

A brief description of the program for a pass that appears on the signup sheet, under the personalization logo.

`requiredPersonalizationFields`

`[string]`

 (Required) 

An array that identifies the signup data required from the user the system shows on the generated signup form.

Possible Values: `PKPassPersonalizationFieldName, PKPassPersonalizationFieldPostalCode, PKPassPersonalizationFieldEmailAddress, PKPassPersonalizationFieldPhoneNumber`

`termsAndConditions`

`string`

A description of the program’s terms and conditions. This string can contain HTML link tags to external content.

If present, this information appears after the user enters their personal information and taps the Next button. The user then has the option to agree to the terms, or to cancel the sign-up process.

## See Also

### Adding personalization information

object Pass.StoreCard

An object that represents groups of fields that show the information for a store card.

