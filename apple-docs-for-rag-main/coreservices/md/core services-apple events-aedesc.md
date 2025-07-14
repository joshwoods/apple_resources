

- Core Services
- Apple Events
-  AEDesc 

Structure

# AEDesc

Stores data and an accompanying descriptor type to formthe basic building block of all Apple Events.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AEDesc
```

## Overview

The Apple Event Manager uses one or more descriptors to constructApple event attributes and parameters, object specifiers, tokens,and many other types of data it works with. (Token is defined in AEDisposeToken(_:).) Adescriptor consists of an opaque data storage container and a descriptortype that identifies the type of the data stored in the descriptor.

The descriptor type is a structure of type `DescType`,which in turn is of data type `ResType`—thatis, a four-character code. Descriptor Type Constants lists the constants for the basic descriptortypes used by the Apple Event Manager. For information about descriptortypes used with object specifiers, see Key Form and Descriptor Type Object Specifier Constants.

### Version-Notes

Prior to Carbon, the AEDataStorage datatype was defined as follows:

typedef Handle AEDataStorage;

## Topics

### Initializers

init()

init(descriptorType: DescType, dataHandle: AEDataStorage!)

### Instance Properties

var dataHandle: AEDataStorage!

An opaque storage type that points to the storagefor the descriptor data. Your application doesn’t access thisdata directly—rather, it calls one of the functions AEGetDescDataSize(_:), AEGetDescData(_:_:_:), or AEReplaceDescData(_:_:_:_:).See AEDataStorage.

var descriptorType: DescType

A four-character code of type DescType that indicates the type ofdata in the structure. See DescType.

