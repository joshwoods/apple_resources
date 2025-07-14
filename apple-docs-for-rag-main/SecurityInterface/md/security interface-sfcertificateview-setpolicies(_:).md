

- Security Interface
- SFCertificateView
-  setPolicies(\_:) 

Instance Method

# setPolicies(\_:)

Specifies the policies to use when evaluating this certificate’s status.

macOS 10.4+

``` source
@MainActor
func setPolicies(_ policies: Any!)
```

## Parameters 

`policies`  

The policy or policies to use. You can pass either a `SecPolicyRef` object or an NSArray (containing one or more objects of type `SecPolicyRef` ) in this parameter. If `policies` is set to nil, the Apple X.509 Basic Policy is used. See Certificate, Key, and Trust Services for a list of policies and object identifiers provided by the AppleX509TP module.

## Discussion

Applications typically display a certificate view in the context of a specific use, such as SSL or S/MIME. You should set only the policy references that apply to your intended use.

## See Also

### Related Documentation

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificate.

### Customizing the Appearance and Behavior of the View

func setDetailsDisclosed(Bool)

Sets whether the certificate details subview is disclosed.

func setDisplayDetails(Bool)

Specifies whether the user can see the certificate details.

func setDisplayTrust(Bool)

Specifies whether the user can see the certificate’s trust settings.

func setEditableTrust(Bool)

Specifies whether the user can edit the certificate’s trust settings.

func setPoliciesDisclosed(Bool)

Specifies whether the trust policy settings subview is disclosed.

