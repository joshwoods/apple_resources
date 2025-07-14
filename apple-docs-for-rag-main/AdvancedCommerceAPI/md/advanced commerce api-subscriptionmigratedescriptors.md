

- Advanced Commerce API
-  SubscriptionMigrateDescriptors 

Object

# SubscriptionMigrateDescriptors

The description and display name of the subscription to migrate to that you manage.

Advanced Commerce API 1.1+

``` source
object SubscriptionMigrateDescriptors
```

## Properties

`description`

description

 (Required) 

The description of the subscription to migrate to. This string doesn’t display to customers.

Maximum length: `45`

`displayName`

displayName

 (Required) 

The display name of the subscription to migrate to. This string displays to customers.

Maximum length: `30`

## See Also

### Migration from the server

Migrate a Subscription to Advanced Commerce API

Migrate a subscription that a customer purchased through In-App Purchase to a subscription you manage using the Advanced Commerce API.

object SubscriptionMigrateRequest

The subscription details you provide to migrate a subscription from In-App Purchase to the Advanced Commerce API, such as descriptors, items, storefront, and more.

object SubscriptionMigrateResponse

A response that contains signed renewal and transaction information after a subscription successfully migrates to the Advanced Commerce API.

object SubscriptionMigrateItem

The SKU, description, and display name to use for a migrated subscription item.

object SubscriptionMigrateRenewalItem

The item information that replaces a migrated subscription item when the subscription renews.

