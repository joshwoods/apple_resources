

- Matter
-  MTROperationalCertificateIssuer 

Protocol

# MTROperationalCertificateIssuer

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
protocol MTROperationalCertificateIssuer
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Instance Properties

var shouldSkipAttestationCertificateValidation: Bool

**Required**

### Instance Methods

func issueOperationalCertificate(forRequest: MTROperationalCSRInfo, attestationInfo: MTRDeviceAttestationInfo, controller: MTRDeviceController, completion: (MTROperationalCertificateChain?, (any Error)?) -> Void)

**Required**

