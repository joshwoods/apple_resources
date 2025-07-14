

- SwiftUI
- AlternatingRowBackgroundBehavior
-  automatic 

Type Property

# automatic

The automatic alternating row background behavior.

macOS 14.0+

``` source
static let automatic: AlternatingRowBackgroundBehavior
```

## Discussion

This defers to default component behavior for alternating row backgrounds. Some components, such as `Table` on macOS, will default to having alternating row backgrounds; while List does not.

## See Also

### Getting alternating row background behavior

static let enabled: AlternatingRowBackgroundBehavior

Alternating rows will be enabled for applicable views.

static let disabled: AlternatingRowBackgroundBehavior

Alternating rows will be disabled for applicable views.

