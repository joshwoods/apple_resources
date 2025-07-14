

- Security Interface
- SFCertificateView
-  policiesDisclosed() 

Instance Method

# policiesDisclosed()

Returns whether the trust policy subview is disclosed.

macOS 10.5+

``` source
@MainActor
func policiesDisclosed() -> Bool
```

## Discussion

The trust policy settings can be shown or hidden depending on whether the user clicks the disclosure triangle. This method returns the state of that disclosure triangle.

## See Also

### Getting Information About the View

func certificate() -> Unmanaged&lt;SecCertificate>!

Returns the certificate currently displayed in the view.

func detailsDisplayed() -> Bool

Indicates if the view currently shows the certificate’s details.

func detailsDisclosed() -> Bool

Returns whether the view currently shows the certificate’s details.

func isTrustDisplayed() -> Bool

Indicates if the view currently shows the certificate’s trust settings.

func isEditable() -> Bool

Indicates if the view allows the user to edit the certificate’s trust.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificate.

