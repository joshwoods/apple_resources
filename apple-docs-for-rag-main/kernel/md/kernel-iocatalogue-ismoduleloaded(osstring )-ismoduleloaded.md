

- Kernel
- IOCatalogue
-  isModuleLoaded(OSString \*) 

# isModuleLoaded(OSString \*)

Reports if a kernel module has been loaded.

``` source
bool isModuleLoaded(
 OSString *moduleName ) const; 
```

## Parameters 

`moduleName`  

Name of the module.

## Return Value

Returns true if the associated kernel module has been loaded into the kernel.

## See Also

### Miscellaneous

addDrivers

Adds an array of driver personalities to the database.

findDrivers(IOService *, SInt32 *)

This is the primary entry point for IOService.

findDrivers(OSDictionary *, SInt32 *)

A more general purpose interface which allows one to retreive driver personalities based the intersection of the 'matching' dictionary and the personality's own property list.

free

Cleans up the database and deallocates memory allocated at initialization. This is never called in normal operation of the system.

getGenerationCount

Get the current generation count of the database.

init

Initializes the database object.

initialize

Creates and initializes the database object and poputates it with in-kernel driver personalities.

isModuleLoaded

Reports if a kernel module has been loaded for a particular personality.

isModuleLoaded(const char *)

Reports if a kernel module has been loaded.

moduleHasLoaded(const char *)

Callback function called after a IOKit dependent kernel module is loaded.

moduleHasLoaded(OSString *)

Callback function called after a IOKit dependent kernel module is loaded.

removeDrivers

Remove driver personalities from the database based on matching information provided.

reset

Return the Catalogue to its initial state.

resetAndAddDrivers

Replace personalities in IOCatalog with those provided.

serialize

Serializes the catalog for transport to the user.

startMatching

Starts an IOService matching thread where matching keys and values are provided by the matching dictionary.

terminateDrivers

Terminates all instances of a driver which match the contents of the matching dictionary. Does not unload module.

terminateDriversForModule(const char *, bool)

Terminates all instances of a driver which depends on a particular module and unloads the module.

terminateDriversForModule(OSString *, bool)

Terminates all instances of a driver which depends on a particular module and unloads the module.

unloadModule

Unloads the reqested module if no driver instances are currently depending on it.

