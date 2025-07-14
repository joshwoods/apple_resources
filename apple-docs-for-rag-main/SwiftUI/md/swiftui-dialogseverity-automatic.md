

- SwiftUI
- DialogSeverity
-  automatic 

Type Property

# automatic

The default dialog severity. Alerts that present an error will use `.critical` and all others will use `.standard`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 13.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let automatic: DialogSeverity
```

## See Also

### Getting severities

static let standard: DialogSeverity

A severity that indicates the dialog is being displayed for the purpose of presenting information to the user.

static let critical: DialogSeverity

A severity that indicates extra attention should be given to the dialog, for example when unexpected data loss may occur as a result of the action taken.

