

- CloudKit JS
- CloudKit.Container
-  discoverAllUserIdentities 

Instance Method

# discoverAllUserIdentities

Fetches all user identities in the current user’s address book.

CloudKit JS 1.0+

``` source
Promise discoverAllUserIdentities();
```

## Return Value

A `Promise` object that resolves to a CloudKit.UserIdentitiesResponse object, or rejects to a CKError object.

## Discussion

Use this method to retrieve information about other users of the app. This method returns information about those users who meet the following criteria:

- The user must be in the current user’s address book.

- The user must have run the app.

- The user must have granted the permission to be discovered for this container.

To get the user identities, use the `users` property in the CloudKit.UserIdentitiesResponse class, which contains an array of CloudKit.UserIdentity dictionaries.

```
myContainer.discoverAllUserIdentities().then(function(response) {
    if(response.hasErrors) {
        // Insert error handling
        throw response.errors[0];
    } else {
        // Insert successfully discovered user code
        var users = response.users;
    }
  });
```

## See Also

### Discovering Users

fetchCurrentUserIdentity

Fetches information about the current user asynchronously.

discoverUserIdentities

Fetches all users in the specified array.

discoverUserIdentityWithEmailAddress

Fetches information about a single user based on the user’s email address.

discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

