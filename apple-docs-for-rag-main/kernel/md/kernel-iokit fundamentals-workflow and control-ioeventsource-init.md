

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  init 

# init

Primary initialiser for the IOEventSource class.

``` source
virtual bool init(
 OSObject *owner,
 IOEventSource::Action action = 0); 
```

## Parameters 

`owner`  

Owner of this instance of an event source. Used as the first parameter of the action callout. Owner will generally be an OSObject it doesn't have to be as no member functions will be called directly in it. It can just be a refcon for a client routine.

`action`  

Pointer to C call out function. Action is a pointer to a C function that gets called when this event source has outstanding work. It will usually be called by the checkForWork member function. The first parameter of the action call out will always be the owner, this allows C++ member functions to be used as actions. Defaults to 0.

## Return Value

true if the inherited classes and this instance initialise successfully.

## See Also

### Miscellaneous

checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

disable

Disable event source.

enable

Enable event source.

getAction

Get'ter for \$link action variable.

getNext

Get'ter for \$link eventChainNext variable.

getWorkLoop

Get'ter for \$link workLoop variable.

isEnabled

Get'ter for \$link enable variable.

onThread

Convenience function for workLoop-\>onThread.

setAction

Set'ter for \$link action variable.

setNext

Set'ter for \$link eventChainNext variable.

setWorkLoop

Set'ter for \$link workLoop variable.

