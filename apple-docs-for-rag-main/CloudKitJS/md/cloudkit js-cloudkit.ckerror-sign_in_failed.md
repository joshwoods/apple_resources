

- CloudKit JS
- CloudKit.CKError
-  SIGN_IN_FAILED 

# SIGN_IN_FAILED

The user failed to sign in.

CloudKit JS 1.0+

``` source
const String SIGN_IN_FAILED;
```

## See Also

### Constants

ACCESS_DENIED

You don’t have permission to access the endpoint, record, zone, or database.

ATOMIC_ERROR

An atomic batch operation failed.

AUTH_PERSIST_ERROR

AUTHENTICATION_FAILED

Authentication was rejected.

AUTHENTICATION_REQUIRED

The request requires authentication but none was provided.

BAD_REQUEST

The request was not valid.

CONFIGURATION_ERROR

CloudKit JS configuration error. For example, no containers are configured.

CONFLICT

The `recordChangeTag` value expired. (Retry the request with the latest tag.)

EXISTS

The resource that you attempted to create already exists.

INTERNAL_ERROR

An internal error occurred.

INVALID_ARGUMENTS

The parameters you provided for this method are invalid.

NETWORK_ERROR

A network error occurred, such as a connection time out.

NOT_FOUND

The resource was not found.

QUOTA_EXCEEDED

If accessing the public database, you exceeded the app’s quota. If accessing the private database, you exceeded the user’s iCloud quota.

SERVICE_UNAVAILABLE

The CloudKit service could not be reached.

