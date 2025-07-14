

- Kernel
- Hardware Families
- Network
- IONetworkMedium
-  getName 

# getName

``` source
virtual const OSSymbol * getName() const; 
```

## Return Value

Returns the name assigned to this medium object.

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

getSpeed

getType

init

Initializes an IONetworkMedium object.

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

