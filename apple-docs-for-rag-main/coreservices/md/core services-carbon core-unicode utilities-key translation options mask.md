

- Core Services
- Carbon Core
- Unicode Utilities
-  Key Translation Options Mask 

# Key Translation Options Mask

Specifies the mask for the bit that controls dead-key processing state.

## Overview

This constant is the currently defined mask for the `keyTranslateOptions` parameter of the function UCKeyTranslate(_:_:_:_:_:_:_:_:_:_:).

## Topics

### Constants

var kUCKeyTranslateNoDeadKeysMask: Int

The mask for the bit that turns off dead-key processing. This prevents setting any new dead-key states, but allows completion of any dead-key states currently in effect.

