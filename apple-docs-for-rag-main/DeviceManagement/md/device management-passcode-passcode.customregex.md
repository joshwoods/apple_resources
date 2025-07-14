

- Device Management
- Passcode
-  Passcode.CustomRegex 

Device Management Profile

# Passcode.CustomRegex

The regex defining the passcode policy.

iOS 4.0+iPadOS 4.0+macOS 10.7+visionOS 2.0+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object Passcode.CustomRegex
```

## Properties

`passwordContentDescription`

Passcode.CustomRegex.PasswordContentDescription

Contains a dictionary of keys for supported OS language IDs (for example, “en-US”), and whose values represent a localized description of the policy enforced by the regular expression. Use the special `default` key can for languages that aren’t contained in the dictionary.

`passwordContentRegex`

`string`

 (Required) 

A regular expression string that the system matches against the password to determine whether it complies with a policy. The regular expression uses the ICU syntax (https://unicode-org.github.io/icu/userguide/strings/regexp.html). The string must not exceed 2048 characters in length.

## Topics

### Profiles

object Passcode.CustomRegex.PasswordContentDescription

Descriptions of the policy, localized to supported locales.

