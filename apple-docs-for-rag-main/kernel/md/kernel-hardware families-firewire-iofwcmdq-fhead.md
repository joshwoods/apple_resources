

- Kernel
- Hardware Families
- FireWire
- IOFWCmdQ
-  fHead 

Instance Property

# fHead

Points to the head of the queue, or NULL if queue is empty

macOS 10.6+

``` source
IOFWCommand *fHead;
```

## See Also

### Fields

fTail

Points to the tail of the queue, or NULL if queue is empty

headChanged

called when head command is changed, or the command itself changes state.

