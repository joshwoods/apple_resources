

- Security Interface
- SFChooseIdentityPanel
-  setDefaultButtonTitle(\_:) 

Instance Method

# setDefaultButtonTitle(\_:)

Customizes the title of the default button.

macOS 10.4+

``` source
@MainActor
func setDefaultButtonTitle(_ title: String!)
```

## Parameters 

`title`  

The new title for the default button. The default title for this button is “OK”.

## Discussion

The default button dismisses the sheet or panel and returns a value of NSOKButton.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setAlternateButtonTitle(String!)

Customizes the title of the alternate button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the optional informative text displayed in the panel.

