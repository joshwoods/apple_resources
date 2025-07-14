

- Core Foundation
- CFBag
-  Predefined Callback Structures 

API Collection

# Predefined Callback Structures

CFBag provides some predefined callbacks for your convenience.

## Topics

### Constants

let kCFTypeBagCallBacks: CFBagCallBacks

let kCFCopyStringBagCallBacks: CFBagCallBacks

Predefined CFBagCallBacks structure containing a set of callbacks appropriate for use when the values in a CFBag are all CFString objects. The bag makes immutable copies of the strings placed into it.

