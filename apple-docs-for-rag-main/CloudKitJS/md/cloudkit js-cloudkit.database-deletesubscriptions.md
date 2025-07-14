

- CloudKit JS
- CloudKit.Database
-  deleteSubscriptions 

Instance Method

# deleteSubscriptions

Deletes one or more subscriptions.

CloudKit JS 1.0+

``` source
Promise deleteSubscriptions(
    CloudKit.Subscription|CloudKit.Subscription[]|String|String[] subscriptions
);
```

## Parameters 

`subscriptions`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.Subscription | A subscription in the database to delete. |
| `CloudKit.Subscription[]` | An array of subscriptions to delete. |
| `String` | The ID of a subscription to delete. |
| `String[]` | An array of IDs of the subscriptions to delete. |

## Return Value

A `Promise` object that resolves to a CloudKit.SubscriptionsResponse object, or rejects to a CKError object.

## Discussion

See Modifying Subscriptions (subscriptions/modify) in CloudKit Web Services Reference.

## See Also

### Subscribing to Changes

saveSubscriptions

Saves one or more subscriptions to record changes.

fetchSubscriptions

Fetches one or more subscriptions.

fetchAllSubscriptions

Fetches all subscriptions in the schema.

