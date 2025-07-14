

- Security Interface
- SFCertificateView
-  setDisplayTrust(\_:) 

Instance Method

# setDisplayTrust(\_:)

Specifies whether the user can see the certificate’s trust settings.

macOS 10.3+

``` source
@MainActor
func setDisplayTrust(_ display: Bool)
```

## Parameters 

`display`  

Pass true to display the trust settings, or false to hide them.

## Discussion

Certificate trust settings are not displayed by default. To show the certificate’s trust settings, you must explicitly set the display value to true. with either this method or the setEditableTrust(_:) method.

## Topics

### Related Documentation

func isTrustDisplayed() -> Bool

Indicates if the view currently shows the certificate’s trust settings.

## See Also

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

