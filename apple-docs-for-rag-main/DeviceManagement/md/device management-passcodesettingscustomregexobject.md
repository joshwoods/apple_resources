

- Device Management
-  PasscodeSettingsCustomRegexObject 

Object

# PasscodeSettingsCustomRegexObject

A regular expression and its description to enforce password compliance.

iOS 15.0+iPadOS 15.0+macOS 13.0+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object PasscodeSettingsCustomRegexObject
```

## Properties

`Description`

PasscodeSettingsCustomRegex_DescriptionObject

A dictionary with supported OS language IDs for the keys (such as `en-US`), and values that represent a localized description of the policy that the regular expression enforces. Use the special `default` key for languages that the dictionary doesn’t contain.

`Regex`

`string`

 (Required) 

A regular expression string to match against the password to determine whether it complies with a policy. The regular expression uses the ICU syntax. The string can’t exceed 2048 characters in length.

## Discussion

Use the simpler passcode settings whenever possible, and rely on regular expression matching only when necessary. Mistakes in regular expressions can lead to frustrating user experiences, such as unsatisfiable passcode policies, or policy descriptions that don’t match the enforced policy.

## See Also

### Supporting Objects

object PasscodeSettingsCustomRegex_DescriptionObject

A dictionary that contains supported OS language IDs for the keys and values that represent a localized description of the policy that the regular expression enforces.

