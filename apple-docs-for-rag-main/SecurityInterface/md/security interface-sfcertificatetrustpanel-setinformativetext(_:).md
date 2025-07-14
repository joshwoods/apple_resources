

- Security Interface
- SFCertificateTrustPanel
-  setInformativeText(\_:) 

Instance Method

# setInformativeText(\_:)

Sets the (optional) informative text displayed in the panel.

macOS 10.5+

``` source
@MainActor
func setInformativeText(_ informativeText: String!)
```

## Parameters 

`informativeText`  

By default, informative text describing the current certificate’s trust status is displayed. Call this method only if your application needs to customize the displayed informative text.

## See Also

### Controlling the Appearance of a Certificate Trust Panel

func informativeText() -> String!

Returns the (optional) informative text currently displayed in the panel.

