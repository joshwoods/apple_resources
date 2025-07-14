

- Virtualization
- VZLinuxRosettaDirectoryShare
-  installRosetta(completionHandler:) 

Type Method

# installRosetta(completionHandler:)

Starts the installation of Rosetta.

macOS 13.0+

``` source
class func installRosetta(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
class func installRosetta() async throws
```

## Parameters 

`completionHandler`  

The completion handler the framework invokes after the request finishes processing.

## Discussion

The completion handler returns an error object that contains information about a problem, or `nil` if the installation completed successfully.

