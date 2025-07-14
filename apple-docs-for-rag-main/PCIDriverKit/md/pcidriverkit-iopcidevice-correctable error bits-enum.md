

- PCIDriverKit
- IOPCIDevice
-  Correctable Error Bits 

API Collection

# Correctable Error Bits

Constants for the bits in the correctable error status register.

## Topics

### Constants

kIOPCICorrectableErrorBitReceiver

The bit number for a receiver error.

kIOPCICorrectableErrorBitBadTLP

The bit number for a bad transaction layer packet error.

kIOPCICorrectableErrorBitBadDLLP

The bit number for a bad DTLP error.

kIOPCICorrectableErrorBitReplayNumRollover

The bit number for an error that requires the retransmission of a packet.

kIOPCICorrectableErrorBitReplayTimerTimeout

The bit number for a timeout error that involves the retransmission of a packet.

kIOPCICorrectableErrorBitAdvisoryNonFatal

The bit number for an advisory error that is not fatal.

kIOPCICorrectableErrorBitCorrectedInternal

The bit number for an error that the device corrected internally.

kIOPCICorrectableErrorBitHeaderLogOverflow

The bit number for a header log overflow error.

## See Also

### Getting Error Codes

Uncorrectable Error Bits

Constants for the bits in the uncorrectable error status register.

