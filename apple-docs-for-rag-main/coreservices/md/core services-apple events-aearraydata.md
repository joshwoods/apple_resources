

- Core Services
- Apple Events
-  AEArrayData 

Structure

# AEArrayData

Stores array information to be put into a descriptor listwith the `AEPutArray` functionor extracted from a descriptor list with the `AEGetArray` function.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AEArrayData
```

## Overview

When your application calls the AEPutArray(_:_:_:_:_:_:) function to put informationinto a descriptor list or the AEGetArray(_:_:_:_:_:_:_:) functionto get information from a descriptor list, it uses an to store theinformation. The type of array depends on the data for the array,as specified by one of the constants described in Data Array Constants.

Array items in Apple event arrays of type `kAEDataArray`, `kAEPackedArray`,or `kAEHandleArray` mustbe factored—that is, contained in a factored descriptor list.Before adding array items to a factored descriptor list, you shouldprovide both a pointer to the data that is common to all array itemsand the size of that common data when you first call AECreateList(_:_:_:_:) to createa factored descriptor list. When you call `AEPutArray` toadd the array data to such a descriptor list, the Apple Event Managerautomatically isolates the common data you specified in the callto `AECreateList`.

When you call `AEGetArray` or `AEPutArray`,you specify a pointer of data type `AEArrayDataPointer` thatpoints to a buffer containing the data for the array.

## Topics

### Instance Properties

var kAEDataArray: Int16

var kAEDescArray: AEDesc

var kAEHandleArray: Handle?

var kAEKeyDescArray: AEKeyDesc

var kAEPackedArray: CChar

### Initializers

init()

init(kAEDataArray: Int16)

init(kAEDescArray: AEDesc)

init(kAEHandleArray: Handle?)

init(kAEKeyDescArray: AEKeyDesc)

init(kAEPackedArray: CChar)

