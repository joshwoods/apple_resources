

- ManagedApp
- ManagedAppPasswordsProvider
-  password(withIdentifier:) 

Instance Method

# password(withIdentifier:)

Provides a password by its identifier.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
func password(withIdentifier identifier: String) async throws(ManagedAppError) -> String
```

## Parameters 

`identifier`  

The identifier of the requested password. This function throws ManagedAppError.invalidIdentifier if the value you supply isn’t currently in identifiers.

## Return Value

The requested password.

## Mentioned in 

Accessing provisioned secrets with identifiers

## Discussion

The MDM server can update the password at any time. After that, identifiers yields a new array of identifiers. Call this method again to obtain the updated password.

The MDM server can change the available passwords at any time. When that happens, the list of valid identifiers updates accordingly. For example, the list of valid identifiers might change between the time that the app accesses identifiers and then calls this method passing in one of its elements. So, the app needs to handle the case that this method throws ManagedAppError.invalidIdentifier.

Important

Avoid storing the password and instead, call this method whenever the app needs the password. For security reasons, avoid logging or displaying the password.

Throws

ManagedAppError.invalidIdentifier if no password exists with the specified identifier.

