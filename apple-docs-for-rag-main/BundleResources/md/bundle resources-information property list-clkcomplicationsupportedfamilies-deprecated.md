

- Bundle Resources
- Information Property List
-  CLKComplicationSupportedFamilies Deprecated

Property List Key

# CLKComplicationSupportedFamilies

The complication families for which the app can provide data.

watchOS 2.0–7.0Deprecated

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Details 

Name  
ClockKit Complication - Supported Families

Type  

array of strings

## Possible Values 

`CLKComplicationFamilyModularSmall`  

`CLKComplicationFamilyModularLarge`  

`CLKComplicationFamilyUtilitarianSmall`  

`CLKComplicationFamilyUtilitarianSmallFlat`  

`CLKComplicationFamilyUtilitarianLarge`  

`CLKComplicationFamilyCircularSmall`  

`CLKComplicationFamilyExtraLarge`  

`CLKComplicationFamilyGraphicCorner`  

`CLKComplicationFamilyGraphicBezel`  

`CLKComplicationFamilyGraphicCircular`  

`CLKComplicationFamilyGraphicRectangular`  

`CLKComplicationFamilyGraphicExtraLarge`  

## Discussion

To add this key to the information property list, enable the desired families in the WatchKit extension’s Complication Configuration settings.

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

WKWatchOnly

A Boolean value indicating whether the app is a watch-only app.

**Name:** App is only available as a standalone watchOS app

PUICAutoLaunchAudioOptOut

A Boolean value that indicates whether a watchOS app should opt out of automatically launching when its companion iOS app starts playing audio content.

**Name:** Opt out of Auto-launch Audio App (Watch)

