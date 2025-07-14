

- Security Interface
- SFChooseIdentityPanel
-  setAlternateButtonTitle(\_:) 

Instance Method

# setAlternateButtonTitle(\_:)

Customizes the title of the alternate button.

macOS 10.4+

``` source
@MainActor
func setAlternateButtonTitle(_ title: String!)
```

## Parameters 

`title`  

The new title for the alternate button. If this method is not called, or if `title` is set to `nil`, the button is not shown.

## Discussion

The alternate button is typically labelled “Cancel”. The alternate button dismisses the sheet or panel and returns a value of NSCancelButton.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

func informativeText() -> String!

Returns the informative text currently displayed in the panel.

func setInformativeText(String!)

Sets the optional informative text displayed in the panel.

