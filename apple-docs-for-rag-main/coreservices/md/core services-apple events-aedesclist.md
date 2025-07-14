

- Core Services
- Apple Events
-  AEDescList 

Type Alias

# AEDescList

A descriptor whose data consists of a list of one or more descriptors.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEDescList = AEDesc
```

## Discussion

Descriptor lists are a key building block of Apple events.

A descriptor list is identical to a descriptor of data type AEDesc —the only difference is that the data in a descriptor list must always consist of a list of other descriptors.

Many Apple Event Manager functions take or return lists of descriptors in descriptor lists. For example, see the functions described in Counting the Items in Descriptor Lists and Getting Items From Descriptor Lists.

The format of the data in the `dataHandle` of the descriptor is private. You can only operate on the contained elements with Apple Event Manager functions, including those described in Counting the Items in Descriptor Lists and Getting Items From Descriptor Lists.

