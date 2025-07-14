

- PackageDescription
- SystemPackageProvider
-  nuget(\_:) 

Type Method

# nuget(\_:)

Creates a system package provider with a list of installable packages for users of the NuGet package manager on Linux or Windows.

SwiftPM 999.0+

``` source
static func nuget(_ packages: [String]) -> SystemPackageProvider
```

## Parameters 

`packages`  

The list of package names.

## Return Value

A package provider.

