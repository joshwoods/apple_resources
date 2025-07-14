

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOEventSource
-  getAction 

# getAction

Get'ter for \$link action variable.

``` source
virtual IOEventSource::Action getAction() const; 
```

## Return Value

value of action.

## See Also

### Miscellaneous

checkForWork

Virtual member function used by IOWorkLoop for work scheduling.

disable

Disable event source.

enable

Enable event source.

getNext

Get'ter for \$link eventChainNext variable.

getWorkLoop

Get'ter for \$link workLoop variable.

init

Primary initialiser for the IOEventSource class.

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

