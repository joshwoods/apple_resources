

- Security Interface
- SFChooseIdentityPanel
-  setInformativeText(\_:) 

Instance Method

# setInformativeText(\_:)

Sets the optional informative text displayed in the panel.

macOS 10.5+

``` source
@MainActor
func setInformativeText(_ informativeText: String!)
```

## Parameters 

`informativeText`  

A string containing a hostname, RFC 822 name (email address), URL, or similar identifier.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setAlternateButtonTitle(String!)

Customizes the title of the alternate button.

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

