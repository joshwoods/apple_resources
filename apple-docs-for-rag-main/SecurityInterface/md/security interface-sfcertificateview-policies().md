

- Security Interface
- SFCertificateView
-  policies() 

Instance Method

# policies()

Returns an array of policies used to evaluate the status of the displayed certificate.

macOS 10.4+

``` source
@MainActor
func policies() -> [Any]!
```

## Discussion

This method returns an autoreleased NSArray containing one or more instances of SecPolicy. The array always contains at least one item (the Apple X.509 Basic policy, if you have never called the setPolicies(_:) method).

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

func policiesDisclosed() -> Bool

Returns whether the trust policy subview is disclosed.

