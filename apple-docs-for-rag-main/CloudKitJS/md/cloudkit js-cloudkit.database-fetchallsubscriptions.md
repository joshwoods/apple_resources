

- CloudKit JS
- CloudKit.Database
-  fetchAllSubscriptions 

Instance Method

# fetchAllSubscriptions

Fetches all subscriptions in the schema.

CloudKit JS 1.0+

``` source
Promise fetchAllSubscriptions();
```

## Return Value

A `Promise` object that resolves to a CloudKit.SubscriptionsResponse object , or rejects to a CKError object.

## Discussion

See Fetching Subscriptions (subscriptions/list) in CloudKit Web Services Reference.

## See Also

### Subscribing to Changes

saveSubscriptions

Saves one or more subscriptions to record changes.

fetchSubscriptions

Fetches one or more subscriptions.

deleteSubscriptions

Deletes one or more subscriptions.

