

- Security Interface
- SFCertificateView
-  isTrustDisplayed() 

Instance Method

# isTrustDisplayed()

Indicates if the view currently shows the certificate’s trust settings.

macOS 10.3+

``` source
@MainActor
func isTrustDisplayed() -> Bool
```

## See Also

### Getting Information About the View

func certificate() -> Unmanaged&lt;SecCertificate>!

Returns the certificate currently displayed in the view.

func detailsDisplayed() -> Bool

Indicates if the view currently shows the certificate’s details.

func detailsDisclosed() -> Bool

Returns whether the view currently shows the certificate’s details.

func isEditable() -> Bool

Indicates if the view allows the user to edit the certificate’s trust.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificate.

func policiesDisclosed() -> Bool

Returns whether the trust policy subview is disclosed.

