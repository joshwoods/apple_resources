

- Core Transferable
- TransferRepresentationVisibility
-  ownProcess 

Type Property

# ownProcess

The visibility level that specifies that the item is visible only within the app that’s the source of the item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static let ownProcess: TransferRepresentationVisibility
```

## See Also

### Specifying transfer visibility

static let all: TransferRepresentationVisibility

The visibility level that specifies that any app or process can access the item.

static let team: TransferRepresentationVisibility

The visibility level that specifies that the item is visible only to apps created by the current app’s development team.

static let group: TransferRepresentationVisibility

The visibility level that specifies that the item is visible only to macOS apps in the same App Group.

