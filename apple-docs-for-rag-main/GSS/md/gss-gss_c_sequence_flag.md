

- GSS
-  GSS_C_SEQUENCE_FLAG 

Global Variable

# GSS_C_SEQUENCE_FLAG

A flag that detects out of sequence messages.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var GSS_C_SEQUENCE_FLAG: Int32 { get }
```

## See Also

### Flags

var GSS_C_DELEG_FLAG: Int32

A flag that permits delegation of the initiator’s credentials by the acceptor.

var GSS_C_MUTUAL_FLAG: Int32

A flag that authenticates the credentials of both initiator and acceptor.

var GSS_C_REPLAY_FLAG: Int32

A flag that detects repeated messages.

var GSS_C_CONF_FLAG: Int32

A flag that makes confidentiality services (that is, encryption) available for transferred messages.

var GSS_C_INTEG_FLAG: Int32

A flag that makes integrity services (that is, cryptographic signatures) available for transferred messages.

var GSS_C_ANON_FLAG: Int32

A flag that ensures the initiator remains anonymous to the acceptor.

var GSS_C_PROT_READY_FLAG: Int32

A flag that provides an early indication of the availability of confidentiality and integrity services.

var GSS_C_TRANS_FLAG: Int32

A flag that indicates that a context can is exportable, for example to transfer it to another process on the same machine.

var GSS_C_DCE_STYLE: Int32

A flag that causes an extra AP reply to be sent from the client back to the server after receiving the server’s AP reply.

var GSS_C_IDENTIFY_FLAG: Int32

A flag that indicates identification of the client by name and ID only.

var GSS_C_EXTENDED_ERROR_FLAG: Int32

A flag that indicates that the client wants to be informed of extended error information.

var GSS_C_DELEG_POLICY_FLAG: Int32

A flag that indicates delegation is permissible if the mechanism policy allows it.

