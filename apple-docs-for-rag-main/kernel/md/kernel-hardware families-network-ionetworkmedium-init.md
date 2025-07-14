

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  init 

# init

Initializes an IONetworkMedium object.

``` source
virtual bool init(
 IOMediumType type, 
 UInt64 speed, 
 UInt32 flags = 0, 
 UInt32 index = 0, 
 const char *name = 0); 
```

## Parameters 

`type`  

The medium type, this value is encoded with bits defined in IONetworkMedium.h.

`speed`  

The maximum (or the only) link speed supported over this medium in units of bits per second.

`flags`  

An optional flag for the medium object. See IONetworkMedium.h for defined flags.

`index`  

An optional index number assigned by the owner. Drivers can use this to store an index to a media table in the driver, or it may map to a driver-defined media type.

`name`  

An optional name assigned to this medium object. If 0, then a name will be created based on the medium type by calling IONetworkMedium::nameForType(). Since the name of the medium is used as a key when inserted into a dictionary, the name chosen must be unique within the scope of the owner.

## Return Value

Returns true on success, false otherwise.

## See Also

### Miscellaneous

addMedium

Adds an IONetworkMedium object to a dictionary.

free

Frees the IONetworkMedium object.

getFlags

getIndex

getKey

getMediumWithIndex

Finds a medium object from a dictionary with a given index.

getMediumWithType

Finds a medium object from a dictionary with a given type.

getName

getSpeed

getType

isEqualTo(const IONetworkMedium *)

Tests for equality between two IONetworkMedium objects.

isEqualTo(const OSMetaClassBase *)

Tests for equality between a IONetworkMedium object and an OSObject.

medium

Factory method that allocates and initializes an IONetworkMedium object.

nameForType

Creates a name that describes a medium type.

removeMedium

Removes an IONetworkMedium object from a dictionary.

serialize

Serializes the IONetworkMedium object.

