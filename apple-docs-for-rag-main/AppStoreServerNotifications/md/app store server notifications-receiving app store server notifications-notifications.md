

- App Store Server Notifications
-  Receiving App Store Server Notifications 

Article

# Receiving App Store Server Notifications

Implement server-side code to receive and parse notification posts.

## Overview

The App Store delivers JSON objects using an HTTP POST to your server for notable in-app purchase events and unreported external purchase tokens. Your server is responsible for parsing, interpreting, and responding to all server-to-server notification posts. For more information about responding, see Responding to App Store Server Notifications.

The body of the POST contains the data elements described in the responseBodyV2 for version 2 notifications, and responseBodyV1 for version 1. Parse them using the following information:

- The version 2 response body, responseBodyV2, contains a signedPayload that’s cryptographically signed by the App Store in JSON Web Signature (JWS) format. The JWS format increases security and enables you to decode and validate the signature on your server. Some notifications include a data object, which has transaction and subscription renewal information that the App Store signs in JWS. The App Store Server API and the StoreKit In-App Purchase API use the same JWS-signed format for transaction and subscription status information. For more information about JWS, see the IETF RFC 7515 specification.

- The version 1 response body, responseBodyV1, is a JSON object. It includes the receipt that contains the most recent in-app purchase transaction for the app. For more information, see the unified_receipt object.

Important

The App Store Server Notifications V1 endpoint and version 1 notifications, notification_type, are deprecated. Instead, implement the App Store Server Notifications V2 endpoint on your server to receive version 2 notifications.

Use the notification type along with the transaction and subscription renewal information to update a user’s service or present promotional offers according to your business logic. For information on handling notifications that contain an external purchase token, see externalPurchaseToken.

## See Also

### Essentials

Enabling App Store Server Notifications

Configure your server and provide an HTTPS URL to receive notifications about in-app purchase events and unreported external purchase tokens.

Responding to App Store Server Notifications

Send HTTP status codes to indicate the success of a notification post.

App Store Server Notifications changelog

Learn about changes to the App Store Server Notifications service.

