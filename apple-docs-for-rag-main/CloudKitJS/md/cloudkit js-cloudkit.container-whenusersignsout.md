

- CloudKit JS
- CloudKit.Container
-  whenUserSignsOut 

Instance Method

# whenUserSignsOut

Returns an object representing a deferred or asynchronous operation that resolves when the user signs out.

CloudKit JS 1.0+

``` source
Promise whenUserSignsOut();
```

## Return Value

A `Promise` object that resolves to `Undefined` when the user signs out, or rejects to a CKError object.

## Discussion

Use the whenUserSignsOut method to call a function when the user signs out.

```
myContainer.whenUserSignsOut().then(function() {
    // The user signed out
});
```

## See Also

### Authenticating Users

setUpAuth

Determines whether a user is signed in and presents an appropriate sign in or sign out button.

whenUserSignsIn

Returns an object representing a deferred or asynchronous operation that resolves when the user signs in.

