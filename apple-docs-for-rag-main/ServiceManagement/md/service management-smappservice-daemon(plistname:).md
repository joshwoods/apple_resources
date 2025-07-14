

- Service Management
- SMAppService
-  daemon(plistName:) 

Type Method

# daemon(plistName:)

Initializes an app service object with a launch daemon with the property list name you provide.

Mac Catalyst 16.0+macOS 13.0+

``` source
class func daemon(plistName: String) -> Self
```

## Parameters 

`plistName`  

The name of the property list corresponding to the SMAppService.

## Return Value

An `SMService` object

## Discussion

The property list name must correspond to a property list in the calling app’s `Contents/Library/LaunchDaemons` directory

## See Also

### Managing apps

class var mainApp: SMAppService

An app service object that corresponds to the main application as a login item.

class func agent(plistName: String) -> Self

Initializes an app service object with a launch agent with the property list name you provide.

class func loginItem(identifier: String) -> Self

Initializes an app service object for a login item corresponding to the bundle with the identifier you provide.

