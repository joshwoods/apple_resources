

- SecureElementCredential
- CredentialSession
- CredentialSession.Credential
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the value by feeding them into the given hasher.

iOS 18.1+iPadOS 18.1+

``` source
func hash(into hasher: inout Hasher)
```

## Discussion

Implement this method to conform to the Hashable protocol. The components you use for hashing must be the same as the components you compare in your type’s `==` operator implementation. Call combine(_:) with each of these components.

Important

Don’t call `finalize()` on `hasher`. It may become a compile-time error.

See Hashable for more information about the concepts and uses of hashing.

