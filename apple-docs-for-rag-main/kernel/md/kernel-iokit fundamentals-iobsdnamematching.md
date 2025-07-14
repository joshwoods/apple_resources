

- Kernel
- IOKit Fundamentals
-  IOBSDNameMatching 

Function

# IOBSDNameMatching

Create a matching dictionary that specifies an IOService match based on BSD device name.

macOS 10.0+

``` source
OSDictionary * IOBSDNameMatching(const char *name);
```

## Parameters 

`masterPort`  

The primary port obtained from IOMasterPort(). Pass kIOMasterPortDefault to look up the default primary port.

`options`  

No options are currently defined.

`bsdName`  

The BSD name, as a const char \*.

## Return Value

The matching dictionary created, is returned on success, or zero on failure. The dictionary is commonly passed to IOServiceGetMatchingServices or IOServiceAddNotification which will consume a reference, otherwise it should be released with CFRelease by the caller.

## Discussion

IOServices that represent BSD devices have an associated BSD name. This function creates a matching dictionary that will match IOService's with a given BSD name.

## See Also

### Driver Registry

IORegistryEntry

The base class for all objects in the registry.

IORegistryIterator

An iterator over the registry.

IOPrintPlane

Registry Utilities

Registry Keys

