

- Advanced Commerce API
-  SubscriptionMigrateResponse 

Object

# SubscriptionMigrateResponse

A response that contains signed renewal and transaction information after a subscription successfully migrates to the Advanced Commerce API.

Advanced Commerce API 1.1+

``` source
object SubscriptionMigrateResponse
```

## Properties

`signedRenewalInfo`

JWSRenewalInfo

 (Required) 

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format, for the migrated subscription.

`signedTransactionInfo`

JWSTransaction

 (Required) 

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format, for the migrated subscription.

## Discussion

This is the response body for the Migrate a Subscription to Advanced Commerce API endpoint.

## See Also

### Migration from the server

Migrate a Subscription to Advanced Commerce API

Migrate a subscription that a customer purchased through In-App Purchase to a subscription you manage using the Advanced Commerce API.

object SubscriptionMigrateRequest

The subscription details you provide to migrate a subscription from In-App Purchase to the Advanced Commerce API, such as descriptors, items, storefront, and more.

object SubscriptionMigrateItem

The SKU, description, and display name to use for a migrated subscription item.

object SubscriptionMigrateRenewalItem

The item information that replaces a migrated subscription item when the subscription renews.

object SubscriptionMigrateDescriptors

The description and display name of the subscription to migrate to that you manage.

