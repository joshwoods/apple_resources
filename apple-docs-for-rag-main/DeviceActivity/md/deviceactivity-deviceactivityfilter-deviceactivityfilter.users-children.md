

- DeviceActivity
- DeviceActivityFilter
- DeviceActivityFilter.Users
-  children 

Type Property

# children

Filters data for the children in the current user’s iCloud family.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static let children: DeviceActivityFilter.Users
```

## Discussion

Only parents and guardians in an iCloud family that are actively managing children via the `FamilyControls` framework have permission to report a child’s device activity data.

