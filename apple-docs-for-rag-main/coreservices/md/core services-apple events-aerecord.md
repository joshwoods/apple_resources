

- Core Services
- Apple Events
-  AERecord 

Type Alias

# AERecord

A descriptor whose data is a list of keyword-specified descriptors.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AERecord = AEDescList
```

## Discussion

The Apple Event Manager provides routines that allow your application to create Apple event records and extract data from them when creating or responding to Apple events. You also work with Apple event records if your application resolves or creates object specifiers. Functions that use Apple event records are described in Apple Event Manager and Apple Event Manager.

The descriptor list of keyword-specified descriptors in an Apple event record must specify Apple event parameters—they cannot specify Apple event attributes. Only descriptor lists of type Apple event can contain both attributes and parameters.

