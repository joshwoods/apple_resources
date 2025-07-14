

- PackageDescription
- PluginPermission
-  PluginPermission.allowNetworkConnections(scope:reason:) 

Case

# PluginPermission.allowNetworkConnections(scope:reason:)

Create a permission to make network connections.

SwiftPM 5.9+

``` source
case allowNetworkConnections(
    scope: PluginNetworkPermissionScope,
    reason: String
)
```

## Parameters 

`scope`  

The scope of the permission.

`reason`  

A reason why the permission is needed. This is shown to the user when permission is sought.

## Discussion

The command plug-in requires permission to make network connections. The `reason` string is shown to the user at the time of request for approval, explaining why the plug-in is requesting access.

## See Also

### Create a permission

case writeToPackageDirectory(reason: String)

Create a permission to modify files in the package’s directory.

