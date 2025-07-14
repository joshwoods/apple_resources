

- CloudKit JS
- CloudKit.Container
-  discoverUserIdentityWithUserRecordName 

Instance Method

# discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

CloudKit JS 1.0+

``` source
Promise discoverUserIdentityWithUserRecordName(
 String userRecordName
);
```

## Parameters 

`userRecordName`  

The name of the user record.

## Return Value

A `Promise` object that resolves to CloudKit.UserIdentitiesResponse object, or rejects to a CKError object.

## Discussion

Use this method to retrieve information about a user for whom you have the corresponding `name` property of the `User` record. The user must meet the following criteria:

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

discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

