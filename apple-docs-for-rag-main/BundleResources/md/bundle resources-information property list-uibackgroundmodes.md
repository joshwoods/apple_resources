

- Bundle Resources
- Information Property List
-  UIBackgroundModes 

Property List Key

# UIBackgroundModes

Services provided by an app that require it to run in the background.

iOS 4.0+iPadOS 4.0+visionOS 1.0+watchOS 4.0+

## Details 

Name  
Required background modes

Type  

array of strings

## Possible Values 

`audio`  

`bluetooth-central`  

`bluetooth-peripheral`  

`external-accessory`  

`fetch`  

`location`  

`nearby-interaction`  

`network-authentication`  

`newsstand-content`  

`processing`  

`push-to-talk`  

`remote-notification`  

`voip`  

## Discussion

To add this key to your Information Property List, enable the Background Modes capability in Xcode. For information on configuring background execution modes and the platforms that support them, see Configuring background execution modes.

## See Also

### Background execution

WKBackgroundModes

The services a watchOS app provides that require it to continue running in the background.

**Name:** Required background modes (Watch)

BGTaskSchedulerPermittedIdentifiers

An array of strings containing developer-specified task identifiers in reverse URL notation.

**Name:** Permitted background task scheduler identifiers

LSBackgroundOnly

A Boolean value indicating whether the app runs only in the background.

**Name:** Application is background only

