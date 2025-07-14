

- Security Interface
- SFCertificateView
-  setDetailsDisclosed(\_:) 

Instance Method

# setDetailsDisclosed(\_:)

Sets whether the certificate details subview is disclosed.

macOS 10.5+

``` source
@MainActor
func setDetailsDisclosed(_ disclosed: Bool)
```

## Parameters 

`disclosed`  

Pass true to open the disclosure triangle and disclose the view, or false to close it and hide the view.

## Discussion

The certificate details can be shown or hidden depending on whether the user clicks the disclosure triangle. This method sets the state of that disclosure triangle and the visibility of the corresponding view.

## See Also

### Customizing the Appearance and Behavior of the View

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

