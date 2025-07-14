

- FamilyControls
- FamilyActivityPicker
-  navigationSubtitle(\_:) 

Instance Method

# navigationSubtitle(\_:)

Configures the view’s subtitle for purposes of navigation.

FamilyControlsSwiftUIMac Catalyst 14.0+macOS 11.0+

``` source
nonisolated
func navigationSubtitle(_ subtitle: Text) -> some View
```

## Parameters 

`subtitle`  

The subtitle to display.

## Discussion

A view’s navigation subtitle is used to provide additional contextual information alongside the navigation title. On macOS, the primary destination’s subtitle is displayed with the navigation title in the titlebar.

