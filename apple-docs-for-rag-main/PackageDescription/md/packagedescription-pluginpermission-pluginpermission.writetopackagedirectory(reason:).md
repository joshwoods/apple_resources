

- PackageDescription
- PluginPermission
-  PluginPermission.writeToPackageDirectory(reason:) 

Case

# PluginPermission.writeToPackageDirectory(reason:)

Create a permission to modify files in the package’s directory.

SwiftPM 5.6+

``` source
case writeToPackageDirectory(reason: String)
```

## Parameters 

`reason`  

A reason why the permission is needed. This is shown to the user when permission is sought.

## Discussion

The command plug-in requires permission to modify the files under the package directory. The `reason` string is shown to the user at the time of request for approval, explaining why the plug-in requests access.

## See Also

### Create a permission

case allowNetworkConnections(scope: PluginNetworkPermissionScope, reason: String)

Create a permission to make network connections.

