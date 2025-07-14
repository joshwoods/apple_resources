

- CloudKit JS
- CloudKit.Container
-  discoverUserIdentities 

Instance Method

# discoverUserIdentities

Fetches all users in the specified array.

CloudKit JS 1.0+

``` source
Promise discoverUserIdentities(
 CloudKit.UserLookupInfo[] userLookupInfos
);
```

## Parameters 

`userLookupInfos`  

Array of information about users to fetch.

## Return Value

A `Promise` object that resolves to a CloudKit.UserIdentitiesResponse object, or rejects to a CKError object.

## Discussion

This method returns information about those users who meet the following criteria:

- The user must be in the current user’s address book.

- The user must have run the app.

- The user must have granted the permission to be discovered for this container.

## See Also

### Discovering Users

fetchCurrentUserIdentity

Fetches information about the current user asynchronously.

discoverAllUserIdentities

Fetches all user identities in the current user’s address book.

discoverUserIdentityWithEmailAddress

Fetches information about a single user based on the user’s email address.

discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

