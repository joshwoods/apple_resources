

- Matter
- MTRDeviceControllerExternalCertificateParameters
-  init(storageDelegate:storageDelegateQueue:uniqueIdentifier:ipk:vendorID:operationalKeypair:operationalCertificate:intermediateCertificate:rootCertificate:) 

Initializer

# init(storageDelegate:storageDelegateQueue:uniqueIdentifier:ipk:vendorID:operationalKeypair:operationalCertificate:intermediateCertificate:rootCertificate:)

iOS 17.6+iPadOS 17.6+Mac Catalyst 17.6+macOS 14.6+tvOS 17.6+visionOS 1.0+watchOS 10.6+

``` source
init(
    storageDelegate: any MTRDeviceControllerStorageDelegate,
    storageDelegateQueue: dispatch_queue_t,
    uniqueIdentifier: UUID,
    ipk: Data,
    vendorID: NSNumber,
    operationalKeypair: any MTRKeypair,
    operationalCertificate: Data,
    intermediateCertificate: Data?,
    rootCertificate: Data
)
```

