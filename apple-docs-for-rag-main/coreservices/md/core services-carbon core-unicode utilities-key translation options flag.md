

- Core Services
- Carbon Core
- Unicode Utilities
-  Key Translation Options Flag 

# Key Translation Options Flag

Indicates the dead-key processing state.

## Overview

Theis constant is the currently defined bit assignment for the `keyTranslateOptions` parameter of the function UCKeyTranslate(_:_:_:_:_:_:_:_:_:_:).

## Topics

### Constants

var kUCKeyTranslateNoDeadKeysBit: Int

The bit number of the bit that turns off dead-key processing. This prevents setting any new dead-key states, but allows completion of any dead-key states currently in effect.

