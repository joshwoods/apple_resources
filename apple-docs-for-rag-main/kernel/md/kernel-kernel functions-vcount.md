

- Kernel
- Kernel Functions
-  vcount 

Function

# vcount

Count total references to a given file, disregarding "kusecount" (event listener, as with O_EVTONLY) references.

macOS 10.5+

``` source
int vcount(vnode_t vp);
```

## Parameters 

`vp`  

The vnode whose references to count.

## Return Value

Count of references.

## Discussion

For a regular file, just return (usecount-kusecount); for device files, return the sum over all vnodes 'v' which reference that device of (usecount(v) - kusecount(v)). Note that this is merely a snapshot and could be invalid by the time the caller checks the result.

