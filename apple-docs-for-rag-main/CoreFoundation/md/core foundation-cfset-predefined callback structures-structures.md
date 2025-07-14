

- Core Foundation
- CFSet
-  Predefined Callback Structures 

API Collection

# Predefined Callback Structures

CFSet provides some predefined callbacks for your convenience.

## Topics

### Constants

let kCFTypeSetCallBacks: CFSetCallBacks

let kCFCopyStringSetCallBacks: CFSetCallBacks

Predefined CFSetCallBacks structure containing a set of callbacks appropriate for use when the values in a set are all CFString objects. The retain callback makes an immutable copy of strings added to the set.

