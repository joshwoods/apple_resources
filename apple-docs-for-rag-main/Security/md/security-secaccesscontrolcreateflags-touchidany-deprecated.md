

- Security
- SecAccessControlCreateFlags
-  touchIDAny Deprecated

Type Property

# touchIDAny

Constraint to access an item with Touch ID for any enrolled fingers.

iOS 9.0–11.3DeprecatediPadOS 9.0–11.3DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12.1–10.13.4DeprecatedtvOS 9.0–11.3DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–4.3Deprecated

``` source
static var touchIDAny: SecAccessControlCreateFlags { get }
```

Deprecated

Use biometryAny instead.

## Discussion

Touch ID must be available and enrolled with at least one finger. The item is still accessible by Touch ID if fingers are added or removed.

