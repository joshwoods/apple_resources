

- App Store Server Notifications
-  responseBodyV1 Deprecated

Object

# responseBodyV1

The response body containing JSON data that the App Store sends in a version 1 server notification.

App Store Server Notifications 1.0–2.8Deprecated

``` source
object responseBodyV1
```

Deprecated

Implement the App Store Server Notifications V2 endpoint on your server to receive version 2 notifications instead.

## Properties

`auto_renew_adam_id`

`string`

Deprecated 

An identifier that App Store Connect generates and the App Store uses to uniquely identify the auto-renewable subscription that the user’s subscription renews. Treat this value as a 64-bit integer.

`auto_renew_product_id`

`string`

Deprecated 

The product identifier of the auto-renewable subscription that the user’s subscription renews.

`auto_renew_status`

`string`

Deprecated 

The current renewal status for an auto-renewable subscription product. Note that these values are the strings `“true”` and `“false”`, and not the strings `“0”` or `“1”` that appear in auto_renew_status in the receipt.

Possible Values: `true, false`

`auto_renew_status_change_date`

`string`

Deprecated 

The time at which the user turned on or off the renewal status for an auto-renewable subscription, in a date-time format similar to the ISO 8601 standard.

`auto_renew_status_change_date_ms`

`string`

Deprecated 

The time at which the user turned on or off the renewal status for an auto-renewable subscription, in UNIX time, in milliseconds. Use this time format to process dates.

`auto_renew_status_change_date_pst`

`string`

Deprecated 

The time at which the user turned on or off the renewal status for an auto-renewable subscription, in Pacific standard time.

`bid`

`string`

Deprecated 

A string that contains the app bundle ID.

`bvrs`

`string`

Deprecated 

A string that contains the app bundle version.

`deprecation`

`string`

Deprecated 

The date that App Store Server Notifications V1 are deprecated. For more information, see App Store Server Notifications changelog.

`environment`

`string`

Deprecated 

The environment for which the App Store generated the receipt.

Possible Values: `Sandbox, PROD`

`expiration_intent`

`integer`

Deprecated 

The reason a subscription expired. This field is only present for an expired auto-renewable subscription. See expiration_intent for more information.

`notification_type`

notification_type

Deprecated 

The subscription event that triggered the notification. See notification_type for the complete list of version 1 notification types.

`original_transaction_id`

`long`

Deprecated 

The original transaction identifier for which App Store Server Notifications sends the notification.

`password`

`string`

Deprecated 

The same value as the shared secret you submit in the `password` field of the App Store Receipt requestBody when validating receipts.

`unified_receipt`

unified_receipt

Deprecated 

An object that contains information about the most recent in-app purchase transactions for the app.

## Mentioned in 

App Store Server Notifications changelog

Receiving App Store Server Notifications

## Discussion

Use the information in the response body to react quickly to changes in your users’ subscription states. The fields available in a notification sent to your server depend on the notification_type, which indicates the event that triggered the notification.

## Topics

### Unified receipt object

object unified_receipt

An object that contains information about the most recent in-app purchase transactions for the app.

## See Also

### Version 1 notifications

App Store Server Notifications V1

Specify your secure server’s URL in App Store Connect to receive version 1 notifications.

Deprecated

type notification_type

The type that describes the in-app purchase event for which the App Store sends the version 1 notification.

Deprecated

