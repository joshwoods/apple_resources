

- Core Services
- Apple Events
-  AEKeyword 

Type Alias

# AEKeyword

A four-character code that uniquely identifies a descriptor in an Apple event record or an Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEKeyword = FourCharCode
```

## Discussion

The Apple Event Manager uniquely identifies the various parts of an Apple event by means of keywords associated with corresponding descriptors. Keywords are arbitrary names, stored as four-character codes of type `AEKeyword`.

A keyword combined with a descriptor forms a keyword-specified descriptor, which is defined by a data structure of type AERemoteProcessResolverContext. The Apple Event Manager also uses keywords for Apple event attributes. Keyword constants used by the Apple Event Manager are defined in Keyword Attribute Constants and Keyword Parameter Constants.

