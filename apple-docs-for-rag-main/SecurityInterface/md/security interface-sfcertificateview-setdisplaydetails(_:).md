

- Security Interface
- SFCertificateView
-  setDisplayDetails(\_:) 

Instance Method

# setDisplayDetails(\_:)

Specifies whether the user can see the certificate details.

macOS 10.4+

``` source
@MainActor
func setDisplayDetails(_ display: Bool)
```

## Parameters 

`display`  

Pass true to display the certificate details, or false to hide them.

## Discussion

For behavioral compatibility with macOS 10.3, certificate details are displayed by default. To hide the details of a certificate, you must explicitly set the display value to false.

## See Also

### Related Documentation

func detailsDisplayed() -> Bool

Indicates if the view currently shows the certificate’s details.

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

