

- HIDDriverKit
- IOUserHIDEventService
-  dispatchStandardGameControllerEvent 

Instance Method

# dispatchStandardGameControllerEvent

DriverKit 21.0+macOS

``` source
kern_return_t dispatchStandardGameControllerEvent(uint64_t timeStamp, IOFixed dpadUp, IOFixed dpadDown, IOFixed dpadLeft, IOFixed dpadRight, IOFixed faceX, IOFixed faceY, IOFixed faceA, IOFixed faceB, IOFixed shoulderL1, IOFixed shoulderR1, IOFixed shoulderL2, IOFixed shoulderR2, IOFixed joystickX, IOFixed joystickY, IOFixed joystickZ, IOFixed joystickRz, bool thumbstickButtonLeft, bool thumbstickButtonRight, IOOptionBits options);
```

