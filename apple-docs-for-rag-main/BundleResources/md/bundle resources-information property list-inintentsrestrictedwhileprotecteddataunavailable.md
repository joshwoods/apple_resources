

- Bundle Resources
- Information Property List
-  INIntentsRestrictedWhileProtectedDataUnavailable 

Property List Key

# INIntentsRestrictedWhileProtectedDataUnavailable

The names of the intent classes your app can’t handle when the user locks the device or the system blocks access to protected data.

iOS 14.0+iPadOS 14.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Intents restricted while locked or protected data unavailable

Type  

array of strings

## Discussion

To specify this information in Xcode, add the intent class name to your app target’s Supported Intents in the Project Editor. Then set the Authentication level to Restricted While Locked or Protected Data Unavailable.

## See Also

### Intents

INIntentsSupported

The names of the intent classes your app handles directly.

**Name:** Intents eligible for in-app handling

INIntentsRestrictedWhileLocked

The names of the intent classes your app can’t handle when the user locks the device.

**Name:** Restricted While Locked

INSupportedMediaCategories

Types of media supported by your app’s media-playing intents.

**Name:** Supported intent media categories

