

- Wallet Passes
- PersonalizationDictionary
-  PersonalizationDictionary.RequiredPersonalizationInfo 

Object

# PersonalizationDictionary.RequiredPersonalizationInfo

An object that contains the user-entered information for a personalized pass.

iOS 10.0+iPadOS 6.0+watchOS 2.0+

``` source
object PersonalizationDictionary.RequiredPersonalizationInfo
```

## Properties

`emailAddress`

`string`

The user-entered email address for the user of the personalized pass.

`familyName`

`string`

The family name for the user of the personalized pass, parsed from the full name. The name can indicate membership in a group.

`fullName`

`string`

The user-entered full name for the user of the personalized pass.

`givenName`

`string`

The given name for the user of the personalized pass, parsed from the full name. The system uses the name to differentiate the individual from other members who share the same family name. In some locales, the given name is also known as a *forename* or *first name*.

`ISOCountryCode`

`string`

The ISO country code. The system sets this key when it’s known; otherwise, it doesn’t include the key.

`phoneNumber`

`string`

The user-entered phone number for the user of the personalized pass.

`postalCode`

`string`

The user-entered postal code for the user of the personalized pass.

