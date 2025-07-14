

- Core Foundation
- CFPlugIn
-  Information Property List Keys 

API Collection

# Information Property List Keys

A plug-in’s information property list can contain these keys used for registering types, factories, and interfaces.

## Topics

### Constants

let kCFPlugInDynamicRegistrationKey: CFString!

Indicates whether a plug-in requires dynamic registration.

let kCFPlugInDynamicRegisterFunctionKey: CFString!

Used to specify a plug-in’s registration function.

let kCFPlugInUnloadFunctionKey: CFString!

Used to specify a plug-in’s unload function.

let kCFPlugInFactoriesKey: CFString!

Used to statically register factory functions.

let kCFPlugInTypesKey: CFString!

Used to statically register the factories that can create each supported type.

