

- Device Management
- SystemMigration
- SystemMigration.CustomBehaviorItem
-  SystemMigration.CustomBehaviorItem.PathsItem 

Device Management Profile

# SystemMigration.CustomBehaviorItem.PathsItem

The custom behavior path dictionary.

macOS 10.12.4+Device Assignment ServicesVPP License Management

``` source
object SystemMigration.CustomBehaviorItem.PathsItem
```

## Properties

`SourcePath`

`string`

 (Required) 

The path to the migrating file or directory on the source system.

`SourcePathInUserHome`

`boolean`

 (Required) 

If `true`, the source path is located within a user home directory.

`TargetPath`

`string`

 (Required) 

The path to the destination file or directory on the target system.

`TargetPathInUserHome`

`boolean`

 (Required) 

If `true`, the target path is located within a user home directory.

## See Also

### Objects

object SystemMigration.CustomBehaviorItem

The custom behavior dictionary.

