

- Security Interface
- SFCertificateView
-  setCertificate(\_:) 

Instance Method

# setCertificate(\_:)

Specifies the certificate that’s displayed in the view.

macOS 10.3+

``` source
@MainActor
func setCertificate(_ certificate: SecCertificate!)
```

## Parameters 

`certificate`  

The new certificate for the view.

## See Also

### Related Documentation

func certificate() -> Unmanaged&lt;SecCertificate>!

Returns the certificate currently displayed in the view.

