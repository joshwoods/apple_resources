

- Service Management
- SMAppService
-  mainApp 

Type Property

# mainApp

An app service object that corresponds to the main application as a login item.

Mac Catalyst 16.0+macOS 13.0+

``` source
class var mainApp: SMAppService { get }
```

## Discussion

Use this `SMAppService` to configure the main app to launch at login.

## See Also

### Managing apps

class func agent(plistName: String) -> Self

Initializes an app service object with a launch agent with the property list name you provide.

class func daemon(plistName: String) -> Self

Initializes an app service object with a launch daemon with the property list name you provide.

class func loginItem(identifier: String) -> Self

Initializes an app service object for a login item corresponding to the bundle with the identifier you provide.

