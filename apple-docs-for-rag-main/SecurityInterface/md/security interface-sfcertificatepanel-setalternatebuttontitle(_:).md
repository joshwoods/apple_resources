

- Security Interface
- SFCertificatePanel
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

## Topics

### Related Documentation

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func runModal(for: SecTrust!, message: String!) -> Int

Displays a modal panel that shows the results of a certificate trust evaluation and that allows the user to edit trust settings.

## See Also

### Customizing the Appearance of the Sheet or Panel

func setDefaultButtonTitle(String!)

Customizes the title of the default button.

func setPolicies(Any!)

Specifies one or more policies that apply to the displayed certificates.

func policies() -> [Any]!

Returns an array of policies used to evaluate the status of the displayed certificates.

