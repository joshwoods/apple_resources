

- Service Management
- SMAppService
-  loginItem(identifier:) 

Type Method

# loginItem(identifier:)

Initializes an app service object for a login item corresponding to the bundle with the identifier you provide.

Mac Catalyst 16.0+macOS 13.0+

``` source
class func loginItem(identifier: String) -> Self
```

## Parameters 

`identifier`  

The bundle identifier of the helper application.

## Return Value

An `SMService` object.

## Discussion

The property list name must correspond to a property list in the calling app’s `Contents/Library/LoginItems` directory

## See Also

### Managing apps

class var mainApp: SMAppService

An app service object that corresponds to the main application as a login item.

class func agent(plistName: String) -> Self

Initializes an app service object with a launch agent with the property list name you provide.

class func daemon(plistName: String) -> Self

Initializes an app service object with a launch daemon with the property list name you provide.

