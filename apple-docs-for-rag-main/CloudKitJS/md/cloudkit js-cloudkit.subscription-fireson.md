

- CloudKit JS
- CloudKit.Subscription
-  firesOn 

Instance Property

# firesOn

An array of keywords that specify the actions that should trigger push notifications. Possible values in the array are: `"create"`, `"update"`, and `"delete"`. This key is not used if `query` is null.

CloudKit JS 1.0+

``` source
attribute String[] firesOn;
```

