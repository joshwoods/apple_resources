

- App Store Server Notifications
-  environment 

Type

# environment

The server environment, either sandbox or production.

App Store Server Notifications 2.0+

``` source
string environment
```

## Possible Values 

`Sandbox`  

Indicates that the notification applies to testing in the sandbox environment.

`Production`  

Indicates that the notification applies to the production environment.

## Discussion

You receive notifications in the sandbox environment when you opt in to receive notifications in the sandbox environment and test your app in the sandbox environment. TestFlight also uses the sandbox environment to send notifications. To opt in to receive notifications, see Enter a URL for App Store Server Notifications. For more information about testing, see Testing at all stages of development with Xcode and the sandbox, and Beta Testing Made Simple with TestFlight.

## See Also

### App metadata and environment

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

type bundleVersion

The version of the build that identifies an iteration of the bundle.

type status

The status of an auto-renewable subscription at the time the App Store signs the notification.

