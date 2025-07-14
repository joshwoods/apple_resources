

- Kernel
- IOKit Fundamentals
- Data Types
- OSOrderedSet
-  setOptions 

Instance Method

# setOptions

macOS 10.11.4+

``` source
virtual unsigned int setOptions(unsigned int options, unsigned int mask, void *context);
```

## Parameters 

`options`  

A bitfield whose values turn the options on (1) or off (0).

`mask`  

A mask indicating which bits in `options` to change. Pass 0 to get the whole current options bitfield without changing any settings.

`context`  

Unused.

## Return Value

The options bitfield as it was before the set operation.

## Discussion

Kernel extensions should not call this function.

Child collections' options are changed only if the receiving ordered set's options actually change.

