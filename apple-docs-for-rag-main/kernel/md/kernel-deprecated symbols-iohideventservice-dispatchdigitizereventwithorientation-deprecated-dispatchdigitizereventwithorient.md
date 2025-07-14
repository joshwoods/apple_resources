

- Kernel
- Deprecated Symbols
- IOHIDEventService
-  dispatchDigitizerEventWithOrientation Deprecated

Instance Method

# dispatchDigitizerEventWithOrientation

macOS 10.12.2–10.15.1Deprecated

``` source
void dispatchDigitizerEventWithOrientation(AbsoluteTime timeStamp, UInt32 transducerID, DigitizerTransducerType type, bool inRange, UInt32 buttonState, IOFixed x, IOFixed y, IOFixed z, IOFixed tipPressure, IOFixed auxPressure, IOFixed twist, DigitizerOrientationType orientationType, IOFixed *orientationParams, UInt32 orientationParamCount, IOOptionBits options);
```

