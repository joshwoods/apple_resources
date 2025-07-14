

- Observation
-  ObservationTracked() 

Macro

# ObservationTracked()

Synthesizes a property for accessors.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@attached(accessor, names: named(init), named(get), named(set), named(_modify)) @attached(peer, names: prefixed(`_`))
macro ObservationTracked()
```

## Overview

The Observation module uses this macro. Its use outside of the framework isn’t necessary.

