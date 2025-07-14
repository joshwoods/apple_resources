

- Bundle Resources
- Information Property List
-  Kernel and drivers 

API Collection

# Kernel and drivers

Configure device drivers provided by the app.

## Topics

### Driver personalities

IOKitPersonalities

One or more groups of attributes that tell the system about the devices your driver supports.

### Kext dependencies

OSBundleCompatibleVersion

The backward limit of compatibility for the current driver.

OSBundleLibraries

The drivers that the system must load before your driver.

### Thunderbolt compatibility

IOPCITunnelCompatible

A Boolean value that indicates whether your driver supports Thunderbolt devices.

## See Also

### Services

Protected resources

Control an app’s access to protected system services and user data.

Data and storage

Regulate documents, URLs, and other kinds of data movement and storage.

App services

Configure services provided by the app, like support for giving directions or using game controllers.

