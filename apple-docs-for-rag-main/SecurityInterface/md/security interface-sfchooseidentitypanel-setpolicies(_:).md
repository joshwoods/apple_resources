

- Security Interface
- SFChooseIdentityPanel
-  setPolicies(\_:) 

Instance Method

# setPolicies(\_:)

Specifies one or more policies that apply to the displayed certificates.

macOS 10.4+

``` source
@MainActor
func setPolicies(_ policies: Any!)
```

## Parameters 

`policies`  

The policies to use when evaluating the certificates’ status. You can pass either a SecPolicy object or an NSArray (containing one or more SecPolicy instances) in this parameter. If `policies` is set to `nil`, the Apple X.509 Basic Policy is used.

## Discussion

The SFChooseIdentityPanel class evaluates trust for the certificates it displays. Applications typically display certificates in the context of a specific use, such as SSL or S/MIME. You should set only the policy references that apply to your intended use. See Certificate, Key, and Trust Services for a list of policies and object identifiers provided by the AppleX509TP Module.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setAlternateButtonTitle(String!)

Customizes the title of the alternate button.

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the optional informative text displayed in the panel.

