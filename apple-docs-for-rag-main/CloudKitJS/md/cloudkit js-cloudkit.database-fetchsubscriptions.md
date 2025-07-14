

- CloudKit JS
- CloudKit.Database
-  fetchSubscriptions 

Instance Method

# fetchSubscriptions

Fetches one or more subscriptions.

CloudKit JS 1.0+

``` source
Promise fetchSubscriptions(
    CloudKit.Subscription|CloudKit.Subscription[]|String|String[] subscriptions
);
```

## Parameters 

`subscriptions`  

Possible values are:

| Type | Description |
|----|----|
| CloudKit.Subscription | A subscription in the database to fetch. |
| `CloudKit.Subscription[]` | An array of subscriptions to fetch. |
| `String` | The ID of a subscription to fetch. |
| `String[]` | An array of IDs of the subscriptions to fetch. |

## Return Value

A `Promise` object that resolves to a CloudKit.SubscriptionsResponse object, or rejects to a CKError object.

## Discussion

See Fetching Subscriptions by Identifier (subscriptions/lookup) in CloudKit Web Services Reference.

## See Also

### Subscribing to Changes

saveSubscriptions

Saves one or more subscriptions to record changes.

fetchAllSubscriptions

Fetches all subscriptions in the schema.

deleteSubscriptions

Deletes one or more subscriptions.

