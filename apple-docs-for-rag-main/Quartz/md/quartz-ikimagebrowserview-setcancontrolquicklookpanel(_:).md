

- Quartz
- IKImageBrowserView
-  setCanControlQuickLookPanel(\_:) 

Instance Method

# setCanControlQuickLookPanel(\_:)

Specifies whether the view can automatically take control of the QuickLook panel.

macOS 10.4+

``` source
@MainActor
func setCanControlQuickLookPanel(_ flag: Bool)
```

## Parameters 

`flag`  

true, if the view can display the QuickLook panel, otherwise false.

## Discussion

When the browser view displays the QuickLook panel it sets itself as the QuickLook datasource. If the browser cells returned by the datasource return items that are URLs or paths, then the QuickLook panel will display the image at that location. Otherwise, the browser cell must implement the doc://com.apple.documentation/documentation/Quartz/qlpreviewitem protocol and return the requested URL for the custom cell.

## See Also

### QuickLook Support

func canControlQuickLookPanel() -> Bool

Returns whether the view can automatically take control of the QuickLook panel.

