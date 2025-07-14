

- Core Foundation
- CFDictionary
-  Predefined Callback Structures 

API Collection

# Predefined Callback Structures

CFDictionary provides some predefined callbacks for your convenience.

## Topics

### Constants

let kCFCopyStringDictionaryKeyCallBacks: CFDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFString objects, which may be mutable and need to be copied in order to serve as constant keys for the values in the dictionary.

let kCFTypeDictionaryKeyCallBacks: CFDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFType-derived objects.

let kCFTypeDictionaryValueCallBacks: CFDictionaryValueCallBacks

Predefined CFDictionaryValueCallBacks structure containing a set of callbacks appropriate for use when the values in a CFDictionary are all CFType-derived objects.

