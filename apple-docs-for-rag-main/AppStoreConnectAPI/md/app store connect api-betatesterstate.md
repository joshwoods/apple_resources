

- App Store Connect API
-  BetaTesterState 

Type

# BetaTesterState

String that describes the state of a beta tester.

App Store Connect API 3.5+

``` source
string BetaTesterState
```

## Possible Values 

`NOT_INVITED`  

`INVITED`  

`ACCEPTED`  

`INSTALLED`  

`REVOKED`  

## Possible values

NOT_INVITED  
The beta tester is not currently invited.

INVITED  
The build of your app is eligible for submission and release on the App Store.

ACCEPTED  
The beta tester has accepted an invite to test a build.

INSTALLED  
The beta tester has installed a build.

REVOKED  
The beta tester chose to stop testing or the beta tester was removed from the app. In both cases the build they installed is not expired. Once the build expires, the system deletes the resource.

## See Also

### Attributes and Relationships

object BetaTester.Attributes

Attributes that describe a beta tester resource.

type BetaInviteType

String that indicates how you offer a beta invitation.

object BetaTester.Relationships

The relationships you included in the request and those on which you can operate.

