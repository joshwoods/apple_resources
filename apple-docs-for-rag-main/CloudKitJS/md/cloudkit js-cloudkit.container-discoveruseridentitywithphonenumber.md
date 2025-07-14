

- CloudKit JS
- CloudKit.Container
-  discoverUserIdentityWithPhoneNumber 

Instance Method

# discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

CloudKit JS 1.0+

``` source
Promise discoverUserIdentityWithPhoneNumber(
 String phoneNumber
);
```

## Parameters 

`phoneNumber`  

The user’s phone number.

## Return Value

A `Promise` object that resolves to CloudKit.UserIdentitiesResponse object, or rejects to a CKError object.

## Discussion

Use this method to get the ID of a user based on the user’s phone number. The user must meet the following criteria:

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

discoverUserIdentityWithEmailAddress

Fetches information about a single user based on the user’s email address.

discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

