

- App Store Server Notifications
-  subtype 

Type

# subtype

A string that provides details about select notification types in version 2.

App Store Server Notifications 2.0+

``` source
string subtype
```

## Possible Values 

`ACCEPTED`  

Applies to the `PRICE_INCREASE` notificationType. A notification with this `subtype` indicates that the customer consented to the subscription price increase if the price increase requires customer consent, or that the system notified them of a price increase if the price increase doesn’t require customer consent.

`AUTO_RENEW_DISABLED`  

Applies to the `DID_CHANGE_RENEWAL_STATUS` notificationType. A notification with this \`subtype indicates that the user disabled subscription auto-renewal, or the App Store disabled subscription auto-renewal after the user requested a refund.

`AUTO_RENEW_ENABLED`  

Applies to the `DID_CHANGE_RENEWAL_STATUS` notificationType. A notification with this `subtype` indicates that the user enabled subscription auto-renewal.

`BILLING_RECOVERY`  

Applies to the `DID_RENEW` notificationType. A notification with this subtype indicates that the expired subscription that previously failed to renew has successfully renewed.

`BILLING_RETRY`  

Applies to the EXPIRED notificationType. A notification with this subtype indicates that the subscription expired because the subscription failed to renew before the billing retry period ended.

`DOWNGRADE`  

Applies to the `DID_CHANGE_RENEWAL_PREF` and `OFFER_REDEEMED` notificationType. A notification with this subtype indicates that the user downgraded their subscription or cross-graded to a subscription with a different duration. Downgrades take effect at the next renewal date.

`FAILURE`  

Applies to the `RENEWAL_EXTENSION` notificationType. A notification with this `subtype` indicates that the subscription-renewal-date extension failed for an individual subscription. For details, see the data object in the responseBodyV2DecodedPayload. For information on the request, see Extend Subscription Renewal Dates for All Active Subscribers.

`GRACE_PERIOD`  

Applies to the `DID_FAIL_TO_RENEW` notificationType. A notification with this subtype indicates that the subscription failed to renew due to a billing issue. Continue to provide access to the subscription during the grace period.

`INITIAL_BUY`  

Applies to the `SUBSCRIBED` notificationType. A notification with this `subtype` indicates that the user purchased the subscription for the first time or that the user received access to the subscription through Family Sharing for the first time.

`PENDING`  

Applies to the `PRICE_INCREASE` notificationType. A notification with this `subtype` indicates that the system informed the user of the subscription price increase, but the user hasn’t accepted it.

`PRICE_INCREASE`  

Applies to the `EXPIRED` notificationType. A notification with this `subtype` indicates that the subscription expired because the user didn’t consent to a price increase.

`PRODUCT_NOT_FOR_SALE`  

Applies to the `EXPIRED` notificationType. A notification with this `subtype` indicates that the subscription expired because the product wasn’t available for purchase at the time the subscription attempted to renew.

`RESUBSCRIBE`  

Applies to the `SUBSCRIBED` notificationType. A notification with this `subtype` indicates that the user resubscribed or received access through Family Sharing to the same subscription or to another subscription within the same subscription group.

`SUMMARY`  

Applies to the `RENEWAL_EXTENSION` notificationType. A notification with this subtype indicates that the App Store server completed your request to extend the subscription renewal date for all eligible subscribers. For the summary details, see the summary object in the responseBodyV2DecodedPayload. For information on the request, see Extend Subscription Renewal Dates for All Active Subscribers.

`UPGRADE`  

Applies to the `DID_CHANGE_RENEWAL_PREF` and `OFFER_REDEEMED` notificationType. A notification with this `subtype` indicates that the user upgraded their subscription or cross-graded to a subscription with the same duration. Upgrades take effect immediately.

`UNREPORTED`  

Applies to the `EXTERNAL_PURCHASE_TOKEN` notificationType. A notification with this `subtype` indicates that Apple created a token for your app but didn’t receive a report. For more information about reporting the token, see externalPurchaseToken.

`VOLUNTARY`  

Applies to the `EXPIRED` notificationType. A notification with this subtype indicates that the subscription expired after the user disabled subscription auto-renewal.

## Mentioned in 

App Store Server Notifications changelog

## Discussion

This `subtype` field is part of the responseBodyV2DecodedPayload, and further describes an event of type notificationType. It’s present only for specific version 2 notifications.

## See Also

### Server notifications version 2

App Store Server Notifications V2

Specify your secure server’s URL in App Store Connect to receive version 2 notifications.

object responseBodyV2

The response body the App Store sends in a version 2 server notification.

object responseBodyV2DecodedPayload

A decoded payload that contains the version 2 notification data.

type notificationType

The type that describes the in-app purchase or external purchase event for which the App Store sends the version 2 notification.

