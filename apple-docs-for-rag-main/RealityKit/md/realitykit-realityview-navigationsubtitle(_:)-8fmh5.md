

- RealityKit
- RealityView
-  navigationSubtitle(\_:) 

Instance Method

# navigationSubtitle(\_:)

Configures the view’s subtitle for purposes of navigation, using a string.

RealityKitSwiftUIMac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func navigationSubtitle(_ subtitle: S) -> some View where S : StringProtocol
```

## Parameters 

`title`  

The subtitle to display.

## Discussion

A view’s navigation subtitle is used to provide additional contextual information alongside the navigation title. On macOS, the primary destination’s subtitle is displayed with the navigation title in the titlebar.

