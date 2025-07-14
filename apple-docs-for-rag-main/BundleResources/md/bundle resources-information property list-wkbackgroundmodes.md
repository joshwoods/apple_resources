

- Bundle Resources
- Information Property List
-  WKBackgroundModes 

Property List Key

# WKBackgroundModes

The services a watchOS app provides that require it to continue running in the background.

watchOS 3.0+

## Details 

Name  
Required background modes (Watch)

Type  

array of strings

## Possible Values 

`workout-processing`  

Allows an active workout session to run in the background.

`self-care`  

Enables extended runtime sessions for brief activities focusing on health or emotional well-being.

`mindfulness`  

Enables extended runtime sessions for silent meditation.

`physical-therapy`  

Enables extended runtime sessions for stretching, strengthening, or range-of-motion exercises.

`alarm`  

Enables extended runtime sessions for smart alarms.

`underwater-depth`  

Enables extended runtime sessions for underwater depth experiences.

## Discussion

To add this key to the Information Property List, enable your WatchKit extension’s Background Modes capability in Xcode.

Important

You can only enable one of the extended runtime session modes (`self-care`, `mindfulness`, `physical-therapy`, or `alarm`). However, you can enable both an extended runtime session mode and the `workout-processing` mode. If you set the background modes using Xcode’s Signing & Capabilities tab, Xcode ensures that these values are set properly.

## See Also

### Related Documentation

Using extended runtime sessions

Create an extended runtime session that continues running your app after the user stops interacting with it.

Running workout sessions

Track a workout on Apple Watch.

### Background execution

UIBackgroundModes

Services provided by an app that require it to run in the background.

**Name:** Required background modes

BGTaskSchedulerPermittedIdentifiers

An array of strings containing developer-specified task identifiers in reverse URL notation.

**Name:** Permitted background task scheduler identifiers

LSBackgroundOnly

A Boolean value indicating whether the app runs only in the background.

**Name:** Application is background only

