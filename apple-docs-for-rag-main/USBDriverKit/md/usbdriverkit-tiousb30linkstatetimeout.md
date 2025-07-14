

- USBDriverKit
-  tIOUSB30LinkStateTimeout 

Enumeration

# tIOUSB30LinkStateTimeout

Constants for the link state timeout values on USB 3.0 devices.

DriverKit 19.0+

``` source
enum tIOUSB30LinkStateTimeout : unsigned int;
```

## Discussion

For information about these constants, see Table 7-12 of the USB 3.0 specification, and sections 7.5.4, 7.5.9, and 7.5.10 of the USB 3.0 specification at http://www.usb.org.

## Topics

### Getting the Link State Timeouts

kIOUSB30LinkStateSSInactiveQuietTimeout

kIOUSB30LinkStateRxDetectQuietTimeout

kIOUSB30LinkStatePollingLFPSTimeout

kIOUSB30LinkStatePollingActiveTimeout

kIOUSB30LinkStatePollingConfigurationTimeout

kIOUSB30LinkStatePollingIdleTimeout

kIOUSB30LinkStateU0LTimeout

kIOUSB30LinkStateU0RecoveryTimeout

kIOUSB30LinkStateU1NoLFPSResponseTimeout

kIOUSB30LinkStateU1PingTimeout

kIOUSB30LinkStateU2NoLFPSResponseTimeout

kIOUSB30LinkStateU3NoLFPSResponseTimeout

kIOUSB30LinkStateU3RxDetectDelay

kIOUSB30LinkStateU3WakeupRetryDelay

kIOUSB30LinKStateU2RxDetectDelay

kIOUSB30LinkStateRecoveryActiveTimeout

kIOUSB30LinkStateRecoveryConfigurationTimeout

kIOUSB30LinkStateRecoveryIdleTimeout

kIOUSB30LinkStateLoopbackExitTimeout

kIOUSB30LinkStateHotResetActiveTimeout

kIOUSB30LinkStatePollingDeadline

kIOUSB30LinkStateSSResumeDeadline

### Enumeration Cases

kIOUSB30LinkStateHotResetDeadline

kIOUSB30LinkStateHotResetExitTimeout

kIOUSB30LinkStateRecoveryDeadline

## See Also

### Timing Parameters

tIOUSB30ResetTimeout

Constants for the reset timeout values on USB 3.0 devices.

tIOUSB30TimingParameters

Constants for USB 3.0 timing parameters.

Timing Parameters

Constants for ping response times.

