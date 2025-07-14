

- App Store Server Notifications
-  externalPurchaseToken 

Object

# externalPurchaseToken

The payload data that contains an external purchase token.

App Store Server Notifications 2.10+

``` source
object externalPurchaseToken
```

## Properties

`externalPurchaseId`

externalPurchaseId

The unique identifier of the token. Use this value to report tokens and their associated transactions in the Send External Purchase Report endpoint.

`tokenCreationDate`

tokenCreationDate

The UNIX time, in milliseconds, when the system created the token.

`appAppleId`

appAppleId

The app Apple ID for which the system generated the token.

`bundleId`

bundleId

The bundle ID of the app for which the system generated the token.

## Mentioned in 

Receiving App Store Server Notifications

App Store Server Notifications changelog

## Discussion

The `externalPurchaseToken` object is part of the responseBodyV2DecodedPayload. It’s present in the payload when the notificationType is `EXTERNAL_PURCHASE_TOKEN`. This notification type applies to apps that use the External Purchase API to offer alternative payment options.

This notification indicates that Apple didn’t receive a report for the token within the time period specified in the Commission, transaction reports, and payments section of the article Using alternative payment options on the App Store in the European Union. To report tokens with or without associated transactions, call the Send External Purchase Report endpoint of the External Purchase Server API from your server.

The `externalPurchaseToken` object in the notification payload is the Base64URL-decoded JSON of the external purchase token your app or website receive when your customer initiates an external purchase. For more information on the external purchase token, see Receiving and decoding external purchase tokens.

## Topics

### External purchase token fields

type externalPurchaseId

The field of an external purchase token that uniquely identifies the token.

type tokenCreationDate

The field of an external purchase token that contains the UNIX date, in milliseconds, when the system created the token.

