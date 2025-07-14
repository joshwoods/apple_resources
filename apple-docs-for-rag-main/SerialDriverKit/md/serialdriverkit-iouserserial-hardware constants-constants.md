

- SerialDriverKit
- IOUserSerial
-  Hardware Constants 

API Collection

# Hardware Constants

Configure your device with the appropriate parity and flow-control options.

## Topics

### Control Bits

PD_RS232_S_DTR

The data-terminal-ready signal.

PD_RS232_S_DSR

The data-set-ready signal.

PD_RS232_S_RTS

The request-to-send signal.

PD_RS232_S_CTS

The clear-to-send signal.

PD_RS232_S_RXO

The receive-data signal.

PD_RS232_S_TXO

The transmit-data signal.

PD_RS232_S_DCD

The data-carrier-detect signal.

### Parity Options

PD_RS232_PARITY_DEFAULT

The default parity setting.

PD_RS232_PARITY_NONE

No parity bit.

PD_RS232_PARITY_ODD

An odd parity bit.

PD_RS232_PARITY_EVEN

An even parity bit.

PD_RS232_PARITY_MARK

The mark state.

PD_RS232_PARITY_SPACE

The space state.

PD_RS232_PARITY_ANY

Discard the parity bit.

## See Also

### Programming the Modem

HwGetModemStatus

Gets the current status of the modem from the hardware.

SetModemStatus

Sets the modem status to the specified values.

HwResetFIFO

Sends a command to reset the specified device queues.

HwSendBreak

Sends a linebreak command to the device.

HwProgramBaudRate

Sets the communication baud rate to the specified value.

HwProgramLatencyTimer

Sets the amount of time to wait before sending the current buffer to the device.

HwProgramMCR

Configure the setings for the device’s modem control register (MCR).

HwProgramUART

Configure the settings for the device’s universal asynchronous receiver/transmitter (UART).

