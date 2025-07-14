

- App Store Server API
-  StatusResponse 

Object

# StatusResponse

A response that contains status information for all of a customer’s auto-renewable subscriptions in your app.

App Store Server API 1.0+

``` source
object StatusResponse
```

## Properties

`data`

`[`SubscriptionGroupIdentifierItem`]`

An array of information for auto-renewable subscriptions, including App Store-signed transaction information and App Store-signed renewal information.

`environment`

environment

The server environment, sandbox or production, in which the App Store generated the response.

`appAppleId`

appAppleId

Your app’s App Store identifier.

`bundleId`

bundleId

Your app’s bundle identifier.

## Topics

### Response Objects and Data Types

object SubscriptionGroupIdentifierItem

Information for auto-renewable subscriptions, including signed transaction information and signed renewal information, for one subscription group.

type environment

The server environment, either sandbox or production.

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

## See Also

### Subscription status

Get All Subscription Statuses

Get the statuses for all of a customer’s auto-renewable subscriptions in your app.

