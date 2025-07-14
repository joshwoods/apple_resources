

- Security
- SecAccessControlCreateFlags
-  touchIDCurrentSet Deprecated

Type Property

# touchIDCurrentSet

Constraint to access an item with Touch ID for currently enrolled fingers.

iOS 9.0–11.3DeprecatediPadOS 9.0–11.3DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12.1–10.13.4DeprecatedtvOS 9.0–11.3DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.3Deprecated

``` source
static var touchIDCurrentSet: SecAccessControlCreateFlags { get }
```

Deprecated

Use biometryCurrentSet instead.

## Discussion

Touch ID must be available and enrolled with at least one finger. The item is invalidated if fingers are added or removed.

