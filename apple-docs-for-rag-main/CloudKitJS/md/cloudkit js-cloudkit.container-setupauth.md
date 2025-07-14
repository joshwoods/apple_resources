

- CloudKit JS
- CloudKit.Container
-  setUpAuth 

Instance Method

# setUpAuth

Determines whether a user is signed in and presents an appropriate sign in or sign out button.

CloudKit JS 1.0+

``` source
Promise setUpAuth();
```

## Return Value

A `Promise` that resolves to a CloudKit.UserIdentity dictionary if an active CloudKit session was found; otherwise, `null`. If an error occurs, a `Promise` object that rejects to a CKError object.

## Discussion

Use the setUpAuth method to determine whether the user is authenticated and to display the appropriate button.

```
var myContainer = CloudKit.getDefaultContainer();

myContainer.setUpAuth().then(function(userIdentity) {
    if(userIdentity) {
        // The user is authenticated
    }
});
```

In the function, use the `userRecordName` property to get the user record name from the CloudKit.UserIdentity parameter.

The setUpAuth method displays the appropriate buttons only if the required DOM elements are found. If the user is not signed in, the method displays a sign-in button; otherwise, it displays a sign-out button.

You can call this method multiple times. For example, call this method to determine if a previous CloudKit session is still valid, and call this method later to display the buttons after you add the required DOM elements.

## See Also

### Authenticating Users

whenUserSignsIn

Returns an object representing a deferred or asynchronous operation that resolves when the user signs in.

whenUserSignsOut

Returns an object representing a deferred or asynchronous operation that resolves when the user signs out.

