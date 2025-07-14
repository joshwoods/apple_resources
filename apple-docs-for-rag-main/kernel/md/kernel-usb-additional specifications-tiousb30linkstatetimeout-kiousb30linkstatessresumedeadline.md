

- Kernel
- Hardware Families
- 
  - Hardware Families
- USB
- Additional Specifications
- tIOUSB30LinkStateTimeout
-  kIOUSB30LinkStateSSResumeDeadline 

Enumeration Case

# kIOUSB30LinkStateSSResumeDeadline

The SuperSpeed resume deadline.

macOS 10.15+

``` source
kIOUSB30LinkStateSSResumeDeadline = (kIOUSB30LinkStateU3WakeupRetryDelay /* accomodation for retimer */ + kIOUSB30LinkStateU3NoLFPSResponseTimeout + kIOUSB30LinkStateRecoveryActiveTimeout + kIOUSB30LinkStateRecoveryConfigurationTimeout + kIOUSB30LinkStateRecoveryIdleTimeout)
```

