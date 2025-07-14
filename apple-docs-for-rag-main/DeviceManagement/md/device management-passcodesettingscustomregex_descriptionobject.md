

- Device Management
-  PasscodeSettingsCustomRegex_DescriptionObject 

Object

# PasscodeSettingsCustomRegex_DescriptionObject

A dictionary that contains supported OS language IDs for the keys and values that represent a localized description of the policy that the regular expression enforces.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object PasscodeSettingsCustomRegex_DescriptionObject
```

## Properties

`ANY`

`string`

A localized description.

## Discussion

An example of a supported language ID is `en-US`.

Use the special `default` key for languages that the dictionary doesn’t contain.

## See Also

### Supporting Objects

object PasscodeSettingsCustomRegexObject

A regular expression and its description to enforce password compliance.

