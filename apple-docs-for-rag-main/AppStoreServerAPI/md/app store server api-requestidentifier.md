

- App Store Server API
-  requestIdentifier 

Type

# requestIdentifier

A string that contains a unique identifier you provide to track each subscription-renewal-date extension request.

App Store Server API 1.1+

``` source
string requestIdentifier
```

## Attributes 

Maximum length: `128`

## Discussion

You provide a `requestIdentifier` in the request body when you call the Extend Subscription Renewal Dates for All Active Subscribers and Extend a Subscription Renewal Date endpoints.

The API returns the same request identifier in its response, so you can match your request with the related response. The App Store Server Notifications V2 also include this request identifier in notifications related to the Extend Subscription Renewal Dates for All Active Subscribers endpoint. For more information, see the `RENEWAL_EXTENSION` notificationType.

To resend the same request due to a timeout or other error, use the same request identifier. Otherwise, create a unique request identifer for each different subscription-renewal-date extension request.

Important

Provide a `UUID` value for the requestIdentifier when calling the Extend Subscription Renewal Dates for All Active Subscribers endpoint.

The maximum string length is 128 characters.

## See Also

### Request data types

type extendByDays

The number of days to extend the subscription renewal date.

type extendReasonCode

The code that represents the reason for the subscription-renewal-date extension.

