

- CarPlay
- CPBarButtonProviding
-  leadingNavigationBarButtons 

Instance Property

# leadingNavigationBarButtons

An array of bar buttons to display on the leading side of the navigation bar.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var leadingNavigationBarButtons: [CPBarButton] { get set }
```

**Required**

## Discussion

The navigation bar displays up to two buttons in the leading space. When including more than two buttons in the array, the system displays only the first two buttons.

## See Also

### Providing Navigation Bar Buttons

var backButton: CPBarButton?

A button to display as the Back button on the navigation bar.

**Required**

var trailingNavigationBarButtons: [CPBarButton]

An array of bar buttons to display on the trailing side of the navigation bar.

**Required**

class CPBarButton

A button for placement in a navigation bar.

class CPMessageComposeBarButton

A button that activates Siri and initiates the compose message flow.

