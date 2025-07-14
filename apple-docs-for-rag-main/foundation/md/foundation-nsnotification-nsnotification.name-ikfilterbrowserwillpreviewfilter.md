

- Foundation
- NSNotification
- NSNotification.Name
-  IKFilterBrowserWillPreviewFilter 

Type Property

# IKFilterBrowserWillPreviewFilter

Posted before showing a filter preview, allowing an application to set the parameters of a filter.

macOS 10.0+

``` source
static let IKFilterBrowserWillPreviewFilter: NSNotification.Name
```

## Discussion

The selected filter is sent as the object in the notification.

## See Also

### Quartz

static let IKFilterBrowserFilterDoubleClick: NSNotification.Name

Posted when the user double-clicks a filter in the filter browser.

static let IKFilterBrowserFilterSelected: NSNotification.Name

Posted when the user clicks a filter name in the filter browser.

static let quartzFilterManagerDidAddFilter: NSNotification.Name

static let quartzFilterManagerDidModifyFilter: NSNotification.Name

static let quartzFilterManagerDidRemoveFilter: NSNotification.Name

static let quartzFilterManagerDidSelectFilter: NSNotification.Name

static let QCCompositionPickerPanelDidSelectComposition: NSNotification.Name

Posted when the user chooses a composition.

Deprecated

static let QCCompositionPickerViewDidSelectComposition: NSNotification.Name

Posted when the user selects a composition in the picker view.

Deprecated

static let QCCompositionRepositoryDidUpdate: NSNotification.Name

Posted whenever the list of compositions in the composition repository is updated.

Deprecated

static let QCViewDidStartRendering: NSNotification.Name

Posted when the view starts rendering.

Deprecated

static let QCViewDidStopRendering: NSNotification.Name

Posted when the view stops rendering.

Deprecated

