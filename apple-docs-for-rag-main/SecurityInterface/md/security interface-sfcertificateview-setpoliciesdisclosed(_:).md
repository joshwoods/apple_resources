

- Security Interface
- SFCertificateView
-  setPoliciesDisclosed(\_:) 

Instance Method

# setPoliciesDisclosed(\_:)

Specifies whether the trust policy settings subview is disclosed.

macOS 10.5+

``` source
@MainActor
func setPoliciesDisclosed(_ disclosed: Bool)
```

## Parameters 

`disclosed`  

Pass true to display the certificate details, or false to hide them.

## Discussion

The trust policy settings can be shown or hidden depending on whether the user clicks the disclosure triangle. This method sets the state of that disclosure triangle and the visibility of the corresponding view.

## See Also

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

