

- ManagedApp
- ManagedAppCertificatesProvider
-  certificate(withIdentifier:) 

Instance Method

# certificate(withIdentifier:)

Provides a certificate by its identifier.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
func certificate(withIdentifier identifier: String) async throws(ManagedAppError) -> SecCertificate
```

## Parameters 

`identifier`  

The identifier of the requested certficate. This function throws ManagedAppError.invalidIdentifier if the value you supply isn’t currently in identifiers.

## Return Value

The requested certificate

## Discussion

The MDM server can update the certificate at any time. After that, identifiers yields a new array of identifiers. Call this method again to obtain the updated certificate.

The MDM server can change the available certificates at any time. When that happens, the list of valid identifiers updates accordingly. For example, the list of valid identifiers might change between the time that the app accesses identifiers and then calls this method passing in one of its elements. So, the app needs to handle the case that this method throws ManagedAppError.invalidIdentifier.

Important

Avoid storing the certificate and instead, call this method whenever the app needs the certificate. For security reasons, avoid logging or displaying the certificate. Even though the cerificate is a “public” certificate, it can contain sensitive information.

Throws

ManagedAppError.invalidIdentifier if no certificate exists with the specified identifier.

