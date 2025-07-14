

- Security Interface
- SFCertificateView
-  setEditableTrust(\_:) 

Instance Method

# setEditableTrust(\_:)

Specifies whether the user can edit the certificate’s trust settings.

macOS 10.3+

``` source
@MainActor
func setEditableTrust(_ editable: Bool)
```

## Parameters 

`editable`  

Pass true if the trust settings should be editable.

## Discussion

For behavioral compatibility with macOS 10.3, this method causes the certificate trust settings to be displayed if they are not currently visible (that is, if setDisplayTrust(_:) is set to false).

## Topics

### Related Documentation

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

## See Also

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setPolicies(Any!)

Specifies the policies to use when evaluating this certificate’s status.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

