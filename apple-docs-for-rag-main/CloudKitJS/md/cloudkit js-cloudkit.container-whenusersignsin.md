

- CloudKit JS
- CloudKit.Container
-  whenUserSignsIn 

Instance Method

# whenUserSignsIn

Returns an object representing a deferred or asynchronous operation that resolves when the user signs in.

CloudKit JS 1.0+

``` source
Promise whenUserSignsIn();
```

## Return Value

A `Promise` object that resolves to a CloudKit.UserIdentity dictionary when the user signs in, or rejects to a CKError object.

## Discussion

Use the whenUserSignsIn method to call a function when the user signs in.

```
myContainer.whenUserSignsIn().then(function(userIdentity) {
    // The user signed in
});
```

## See Also

### Authenticating Users

setUpAuth

Determines whether a user is signed in and presents an appropriate sign in or sign out button.

whenUserSignsOut

Returns an object representing a deferred or asynchronous operation that resolves when the user signs out.

