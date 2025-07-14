

- System Extensions
- OSSystemExtensionsWorkspace
-  systemExtensions(forApplicationWithBundleID:) 

Instance Method

# systemExtensions(forApplicationWithBundleID:)

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+

``` source
func systemExtensions(forApplicationWithBundleID bundleID: String) throws -> Set
```

## Parameters 

`bundleID`  

BundleIdentifier of the application containing the system extension(s)

## Return Value

A set of system extension property objects on success, nil otherwise.

