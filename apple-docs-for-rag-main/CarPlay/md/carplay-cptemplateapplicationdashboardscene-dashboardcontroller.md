

- CarPlay
- CPTemplateApplicationDashboardScene
-  dashboardController 

Instance Property

# dashboardController

The controller that manages the dashboard scene’s shortcut buttons.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
@MainActor
var dashboardController: CPDashboardController { get }
```

## Discussion

Use this property to access the controller CarPlay creates when it connects your navigation app’s dashboard scene. You use this controller to manage the shortcut buttons CarPlay displays in the dashboard when there’s no active navigation session.

## See Also

### Accessing the Dashboard Controller

class CPDashboardController

A controller that provides shortcut buttons for the CarPlay Dashboard.

