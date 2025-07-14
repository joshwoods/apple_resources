

- CloudKit JS
- CloudKit.Container
-  discoverUserIdentityWithEmailAddress 

Instance Method

# discoverUserIdentityWithEmailAddress

Fetches information about a single user based on the user’s email address.

CloudKit JS 1.0+

``` source
Promise discoverUserIdentityWithEmailAddress(
 String emailAddress
);
```

## Parameters 

`emailAddress`  

The user’s email address.

## Return Value

A `Promise` object that resolves to CloudKit.UserIdentitiesResponse object, or rejects to a CKError object.

## Discussion

Use this method to get the ID of a user based on the user’s email address. The user must meet the following criteria:

- The user must be in the current user’s address book.

- The user must have run the app.

- The user must have granted the permission to be discovered for this container.

## See Also

### Discovering Users

fetchCurrentUserIdentity

Fetches information about the current user asynchronously.

discoverAllUserIdentities

Fetches all user identities in the current user’s address book.

discoverUserIdentities

Fetches all users in the specified array.

discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

