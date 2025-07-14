

- Security Interface
- SFChooseIdentityPanel
-  policies() 

Instance Method

# policies()

Returns an array of policies used to evaluate the status of the displayed certificates.

macOS 10.4+

``` source
@MainActor
func policies() -> [Any]!
```

## Discussion

This method returns an autoreleased NSArray containing one or more objects of type SecPolicy , as set by a previous setPolicies(_:) call, or the Apple X.509 Basic Policy if setPolicies(_:) has not been called. See Certificate, Key, and Trust Services in Certificate, Key, and Trust Services for a list of policies and object identifiers provided by the AppleX509TP Module.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setAlternateButtonTitle(String!)

Customizes the title of the alternate button.

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the optional informative text displayed in the panel.

