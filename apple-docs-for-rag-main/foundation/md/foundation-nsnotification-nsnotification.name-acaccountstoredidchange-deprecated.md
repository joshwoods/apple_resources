

- Foundation
- NSNotification
- NSNotification.Name
-  ACAccountStoreDidChange Deprecated

Type Property

# ACAccountStoreDidChange

Posted when the accounts managed by this account store changed in the database.

iOS 5.0–14.0DeprecatediPadOS 5.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0Deprecated

``` source
static let ACAccountStoreDidChange: NSNotification.Name
```

Deprecated

Public notification deprecated. Internal clients, see private header for replacement

## Discussion

The notification sent if an account is saved or removed locally or externally. If you receive this notification, you should refetch all account objects.

There’s no `userInfo` dictionary associated with this notification.

