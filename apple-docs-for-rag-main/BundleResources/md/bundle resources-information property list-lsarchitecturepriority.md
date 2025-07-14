

- Bundle Resources
- Information Property List
-  LSArchitecturePriority 

Property List Key

# LSArchitecturePriority

An array of the architectures that the app supports, arranged according to their preferred usage.

macOS 10.1+

## Details 

Name  
Architecture priority

Type  

array of strings

## Possible Values 

`i386`  

The 32-bit Intel architecture.

`x86_64`  

The 64-bit Intel architecture.

`arm64`  

The 64-bit ARM architecture.

`arm64e`  

The 64-bit ARM architecture with pointer authentication code support.

## Attributes 

Default: `i386`

## Discussion

Use this key to prioritize the execution of a specific architecture in a universal binary. This key contains an array of strings, with each string specifying the name of a supported architecture. The order of the strings in the array represents your preference for executing the app. For example, if you specify the `x86_64` architecture first for a universal app, the system runs that app under Rosetta translation on Apple silicon. For more information about Rosetta translation, see About the Rosetta translation environment.

## See Also

### Launch conditions

UIRequiredDeviceCapabilities

The device-related features that your app requires to run.

**Name:** Required device capabilities

LSMultipleInstancesProhibited

A Boolean value indicating whether more than one user can launch the app simultaneously.

**Name:** Application prohibits multiple instances

LSRequiresNativeExecution

A Boolean value that indicates whether to require the execution of the app’s native architecture when multiple architectures are available.

**Name:** Application requires native environment

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

