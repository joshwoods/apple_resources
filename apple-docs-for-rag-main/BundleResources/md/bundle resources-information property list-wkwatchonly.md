

- Bundle Resources
- Information Property List
-  WKWatchOnly 

Property List Key

# WKWatchOnly

A Boolean value indicating whether the app is a watch-only app.

watchOS 6.0+

## Details 

Name  
App is only available as a standalone watchOS app

Type  

boolean

## Discussion

Xcode automatically includes this key in the WatchKit extension’s information property list and sets its value to `YES` when you create a project using the Watch App template. When you set the value of this key to `YES`, the app is only available on Apple Watch, with no related iOS app.

## See Also

### Launch conditions

UIRequiredDeviceCapabilities

The device-related features that your app requires to run.

**Name:** Required device capabilities

LSMultipleInstancesProhibited

A Boolean value indicating whether more than one user can launch the app simultaneously.

**Name:** Application prohibits multiple instances

LSArchitecturePriority

An array of the architectures that the app supports, arranged according to their preferred usage.

**Name:** Architecture priority

LSRequiresNativeExecution

A Boolean value that indicates whether to require the execution of the app’s native architecture when multiple architectures are available.

**Name:** Application requires native environment

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

WKRunsIndependentlyOfCompanionApp

A Boolean value indicating whether the user can install and run the watchOS app independently of its iOS companion app.

**Name:** App can run independently of companion iPhone app

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

**Name:** Opt out of Auto-launch Audio App (Watch)

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

**Name:** ClockKit Complication - Supported Families

Deprecated

