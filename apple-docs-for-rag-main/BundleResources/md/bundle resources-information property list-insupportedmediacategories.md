

- Bundle Resources
- Information Property List
-  INSupportedMediaCategories 

Property List Key

# INSupportedMediaCategories

Types of media supported by your app’s media-playing intents.

iOS 14.0+iPadOS 14.0+tvOS 14.0+visionOS 1.0+

## Details 

Name  
Supported intent media categories

Type  

array of strings

## Possible Values 

`INMediaCategoryAudiobooks`  

Audiobooks

`INMediaCategoryMusic`  

Music

`INMediaCategoryGeneral`  

General

`INMediaCategoryPodcasts`  

Podcasts

`INMediaCategoryRadio`  

Radio

## Discussion

Specify one or more media categories to allow Siri to invoke your app’s intent handling when a user asks to play media. Use `INMediaCategoryGeneral` for media that doesn’t fit into any of the other categories, like white noise or sound effects.

To specify this information in Xcode, add doc://com.apple.documentation/documentation/sirikit/inplaymediaintent to your app’s list of Supported Intents. Then select the relevant media types in the list that appears.

## See Also

### Intents

INIntentsSupported

The names of the intent classes your app handles directly.

**Name:** Intents eligible for in-app handling

INIntentsRestrictedWhileLocked

The names of the intent classes your app can’t handle when the user locks the device.

**Name:** Restricted While Locked

INIntentsRestrictedWhileProtectedDataUnavailable

The names of the intent classes your app can’t handle when the user locks the device or the system blocks access to protected data.

**Name:** Intents restricted while locked or protected data unavailable

