

- Observation
-  Observable() 

Macro

# Observable()

Defines and implements conformance of the Observable protocol.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(member, names: named(_$observationRegistrar), named(access), named(withMutation)) @attached(memberAttribute) @attached(extension, conformances: Observable) macro Observable()
```

## Mentioned in 

Applying Macros

## Overview

This macro adds observation support to a custom type and conforms the type to the Observable protocol. For example, the following code applies the `Observable` macro to the type `Car` making it observable:

```
@Observable 
class Car {
   var name: String = ""
   var needsRepairs: Bool = false

   init(name: String, needsRepairs: Bool = false) {
       self.name = name
       self.needsRepairs = needsRepairs
   }
}
```

## See Also

### Observable conformance

protocol Observable

A type that emits notifications to observers when underlying data changes.

