

- Bundle Resources
- Information Property List
-  LSRequiresNativeExecution 

Property List Key

# LSRequiresNativeExecution

A Boolean value that indicates whether to require the execution of the app’s native architecture when multiple architectures are available.

macOS 10.0+

## Details 

Name  
Application requires native environment

Type  

boolean

## Discussion

The presence of this key causes the system to choose a native architecture over one that requires translation. For example, this key prevents the system from using the Rosetta translation process to execute the Intel portion of a universal app on Apple silicon.

If your app’s binary supports only the Intel architecture and you link the app against the macOS 11 SDK or later, the inclusion of this key prevents your app from running on Apple silicon. If you link the app against an earlier macOS SDK, the app runs under Rosetta translation.

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

WKPrefersNetworkUponForeground

A Boolean value that indicates whether an app requires network access on launch.

WKRunsIndependentlyOfCompanionApp

A Boolean value indicating whether the user can install and run the watchOS app independently of its iOS companion app.

**Name:** App can run independently of companion iPhone app

WKWatchOnly

A Boolean value indicating whether the app is a watch-only app.

**Name:** App is only available as a standalone watchOS app

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

**Name:** Opt out of Auto-launch Audio App (Watch)

CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

**Name:** ClockKit Complication - Supported Families

Deprecated

