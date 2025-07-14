

- CloudKit JS
- CloudKit.Container
-  fetchCurrentUserIdentity 

Instance Method

# fetchCurrentUserIdentity

Fetches information about the current user asynchronously.

CloudKit JS 1.0+

``` source
Promise fetchCurrentUserIdentity();
```

## Return Value

A `Promise` object that resolves to a CloudKit.UserIdentity dictionary if the current user is found, or rejects to a CKError object.

## Discussion

If the current user is discoverable, the CloudKit.UserIdentity dictionary contains a `nameComponents` key that you can use to get the user’s first and last name.

## See Also

### Discovering Users

discoverAllUserIdentities

Fetches all user identities in the current user’s address book.

discoverUserIdentities

Fetches all users in the specified array.

discoverUserIdentityWithEmailAddress

Fetches information about a single user based on the user’s email address.

discoverUserIdentityWithPhoneNumber

Fetches information about a single user based on the user’s phone number.

discoverUserIdentityWithUserRecordName

Fetches information about a single user using the record name.

