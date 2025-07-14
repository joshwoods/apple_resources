

- App Store Server Notifications
-  data 

Object

# data

The payload data that contains app metadata and the signed renewal and transaction information.

App Store Server Notifications 2.0+

``` source
object data
```

## Properties

`appAppleId`

appAppleId

The unique identifier of the app that the notification applies to. This property is available for apps that users download from the App Store. It isn’t present in the sandbox environment.

`bundleId`

bundleId

The bundle identifier of the app.

`bundleVersion`

bundleVersion

The version of the build that identifies an iteration of the bundle.

`consumptionRequestReason`

consumptionRequestReason

The reason the customer requested the refund. This field appears only for `CONSUMPTION_REQUEST` notifications, which the server sends when a customer initiates a refund request for a consumable in-app purchase or auto-renewable subscription.

`environment`

environment

The server environment that the notification applies to, either `sandbox` or `production`.

`signedRenewalInfo`

JWSRenewalInfo

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format. This field appears only for notifications that apply to auto-renewable subscriptions.

`signedTransactionInfo`

JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) format.

`status`

status

The status of an auto-renewable subscription as of the `signedDate` in the responseBodyV2DecodedPayload. This field appears only for notifications sent for auto-renewable subscriptions.

## Mentioned in 

App Store Server Notifications changelog

Receiving App Store Server Notifications

## Discussion

The `data` object is part of the responseBodyV2DecodedPayload. It’s present in the payload for notificationType values related to in-app purchases, except for the `RENEWAL_EXTENSION` notification type with a `SUMMARY` subtype, and the `EXTERNAL_PURCHASE_TOKEN` notification type.

Use the notification type along with the transaction and subscription renewal information in the `data` object to update a user’s service or present promotional offers according to your business logic.

## Topics

### App metadata and environment

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type bundleVersion

The version of the build that identifies an iteration of the bundle.

type environment

The server environment, either sandbox or production.

type status

The status of an auto-renewable subscription at the time the App Store signs the notification.

### JWS transaction and renewal info

type JWSRenewalInfo

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

object JWSRenewalInfoDecodedPayload

A decoded payload containing subscription renewal information for an auto-renewable subscription.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

object JWSTransactionDecodedPayload

A decoded payload that contains transaction information.

### Consumption request info

type consumptionRequestReason

The customer-provided reason for a refund request.

## See Also

### Response objects for in-app purchases

object summary

The payload data for a subscription-renewal-date extension notification.

