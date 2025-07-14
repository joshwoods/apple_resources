

- Accounts
-  ACErrorClientPermissionDenied 

Global Variable

# ACErrorClientPermissionDenied

Error code that indicates the client doesn’t have access to the requested data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.8+

``` source
var ACErrorClientPermissionDenied: ACErrorCode { get }
```

## See Also

### Errors

var ACErrorUnknown: ACErrorCode

Error code that indicates an unknown error occurred.

var ACErrorAccountMissingRequiredProperty: ACErrorCode

Error code that indicates an account wasn’t saved because a required property is missing.

var ACErrorAccountAuthenticationFailed: ACErrorCode

Error code that indicates an account wasn’t saved because authentication of its credential failed.

var ACErrorAccountTypeInvalid: ACErrorCode

Error code that indicates an account wasn’t saved because its account type is invalid.

var ACErrorAccountAlreadyExists: ACErrorCode

Error code that indicates an account wasn’t added because it already exists.

var ACErrorAccountNotFound: ACErrorCode

Error code that indicates an account wasn’t deleted because it couldn’t be found.

var ACErrorPermissionDenied: ACErrorCode

Error code that indicates the operation failed because the application doesn’t have permission to perform the operation.

var ACErrorAccessInfoInvalid: ACErrorCode

Error code that indicates the client’s access info dictionary has incorrect or missing values.

var ACErrorAccessDeniedByProtectionPolicy: ACErrorCode

Error code that indicates due to the current protection policy, the credentials couldn’t be fetched.

var ACErrorCredentialNotFound: ACErrorCode

Error code that indicates no credentials were found.

var ACErrorFetchCredentialFailed: ACErrorCode

Error code that indicates the credentials couldn’t be fetched from Keychain.

var ACErrorStoreCredentialFailed: ACErrorCode

Error code that indicates the credentials couldn’t be stored in Keychain.

var ACErrorRemoveCredentialFailed: ACErrorCode

Error code that indicates the credentials couldn’t be removed from Keychain.

var ACErrorUpdatingNonexistentAccount: ACErrorCode

Error code that indicates an account save failed because the account being updated has been removed.

var ACErrorInvalidClientBundleID: ACErrorCode

Error code that indicates the client making the request doesn’t have a valid bundle ID.

