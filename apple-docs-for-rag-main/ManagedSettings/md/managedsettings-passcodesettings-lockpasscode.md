

- ManagedSettings
- PasscodeSettings
-  lockPasscode 

Type Property

# lockPasscode

The metadata for the setting that prevents the user from changing their passcode.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
static let lockPasscode: SettingMetadata
```

## Discussion

Use `lockPasscode` to access metadata for lockPasscode. The default value is `false`.

## See Also

### Blocking Passcode Changes

var lockPasscode: Bool?

A Boolean value that indicates whether to prevent changing the device passcode.

