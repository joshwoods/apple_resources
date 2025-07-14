

- Kernel
- Hardware Families
- FireWire
- IOFWCmdQ
-  fTail 

Instance Property

# fTail

Points to the tail of the queue, or NULL if queue is empty

macOS 10.6+

``` source
IOFWCommand *fTail;
```

## See Also

### Fields

fHead

Points to the head of the queue, or NULL if queue is empty

headChanged

called when head command is changed, or the command itself changes state.

