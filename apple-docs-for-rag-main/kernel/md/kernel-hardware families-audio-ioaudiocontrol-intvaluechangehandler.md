

- Kernel
- Hardware Families
- Audio
- IOAudioControl
-  IntValueChangeHandler 

# IntValueChangeHandler

Handler function used to make a notification when a value is to be changed.

``` source
typedef IOReturn ( *IntValueChangeHandler)(
   OSObject *target,
   IOAudioControl *audioControl,
   SInt32 oldValue,
   SInt32 newValue);
```

## Parameters 

`target`  

Reference supplied when the handler was registered.

`audioControl`  

The IOAudioControl that is changing.

`oldValue`  

The old value of the control.

`newValue`  

The new value the control is being changed to.

## Return Value

Must return kIOReturnSuccess when the hardware is successfully updated.

