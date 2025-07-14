

- Open Directory
-  ODFrameworkErrors 

Structure

# ODFrameworkErrors

Mac CatalystmacOS

``` source
struct ODFrameworkErrors
```

## Topics

### Constants

var kODErrorCredentialsAccountDisabled: ODFrameworkErrors

The account is disabled.

var kODErrorCredentialsAccountExpired: ODFrameworkErrors

The account is expired.

var kODErrorCredentialsAccountInactive: ODFrameworkErrors

The account is inactive.

var kODErrorCredentialsAccountNotFound: ODFrameworkErrors

The authentication server could not find the provided account.

var kODErrorCredentialsInvalid: ODFrameworkErrors

The provided credentials are invalid with the current node.

var kODErrorCredentialsInvalidComputer: ODFrameworkErrors

The account is not permitted to log into this computer.

var kODErrorCredentialsInvalidLogonHours: ODFrameworkErrors

The logon attempt was not within set logon hours.

var kODErrorCredentialsMethodNotSupported: ODFrameworkErrors

The extended authentication method is not supported.

var kODErrorCredentialsNotAuthorized: ODFrameworkErrors

The operation, such as changing a password, is not permitted with current privileges.

var kODErrorCredentialsOperationFailed: ODFrameworkErrors

The requested operation failed.

var kODErrorCredentialsParameterError: ODFrameworkErrors

An invalid parameter was provided.

var kODErrorCredentialsPasswordChangeRequired: ODFrameworkErrors

The password must be changed.

var kODErrorCredentialsPasswordChangeTooSoon: ODFrameworkErrors

The password was changed too recently to be changed again.

var kODErrorCredentialsPasswordExpired: ODFrameworkErrors

The password has expired and must be changed.

var kODErrorCredentialsPasswordNeedsDigit: ODFrameworkErrors

The provided password needs at least one digit.

var kODErrorCredentialsPasswordNeedsLetter: ODFrameworkErrors

The provided password needs at least one letter.

var kODErrorCredentialsPasswordQualityFailed: ODFrameworkErrors

The provided password did not meet minimum quality requirements.

var kODErrorCredentialsPasswordTooLong: ODFrameworkErrors

The provided password is too long.

var kODErrorCredentialsPasswordTooShort: ODFrameworkErrors

The provided password is too short.

var kODErrorCredentialsPasswordUnrecoverable: ODFrameworkErrors

The password could not be recovered from the authentication database.

var kODErrorCredentialsServerCommunicationError: ODFrameworkErrors

The authentication server encountered a communication error.

var kODErrorCredentialsServerError: ODFrameworkErrors

The authentication server encountered an error.

var kODErrorCredentialsServerNotFound: ODFrameworkErrors

The authentication server could not be found.

var kODErrorCredentialsServerTimeout: ODFrameworkErrors

The authentication server timed out.

var kODErrorCredentialsServerUnreachable: ODFrameworkErrors

The authentication server could not be reached.

var kODErrorDaemonError: ODFrameworkErrors

The daemon has encountered an undefined error.

var kODErrorNodeConnectionFailed: ODFrameworkErrors

The node connection failed.

var kODErrorNodeDisabled: ODFrameworkErrors

var kODErrorNodeUnknownHost: ODFrameworkErrors

The host provided is invalid.

var kODErrorNodeUnknownName: ODFrameworkErrors

The node name provided does not exist and cannot be opened.

var kODErrorNodeUnknownType: ODFrameworkErrors

The node type provided is not a known value.

var kODErrorPluginError: ODFrameworkErrors

A plug-in has encountered an undefined error.

var kODErrorPluginOperationNotSupported: ODFrameworkErrors

The plug-in does not support the requested operation.

var kODErrorPluginOperationTimeout: ODFrameworkErrors

var kODErrorPolicyOutOfRange: ODFrameworkErrors

var kODErrorPolicyUnsupported: ODFrameworkErrors

var kODErrorQueryInvalidMatchType: ODFrameworkErrors

An invalid match type was provided in the query.

var kODErrorQuerySynchronize: ODFrameworkErrors

A query synchronization has been initiated.

var kODErrorQueryTimeout: ODFrameworkErrors

The query timed out.

var kODErrorQueryUnsupportedMatchType: ODFrameworkErrors

An unsupported match type was provided in the query.

var kODErrorRecordAlreadyExists: ODFrameworkErrors

The record create failed because the record already exists.

var kODErrorRecordAttributeNotFound: ODFrameworkErrors

The requested attribute could not be found in the record.

var kODErrorRecordAttributeUnknownType: ODFrameworkErrors

The attribute type is unknown.

var kODErrorRecordAttributeValueNotFound: ODFrameworkErrors

The requested attribute value could not be found in the record.

var kODErrorRecordAttributeValueSchemaError: ODFrameworkErrors

The attribute value does not meet schema requirements.

var kODErrorRecordInvalidType: ODFrameworkErrors

var kODErrorRecordNoLongerExists: ODFrameworkErrors

var kODErrorRecordParameterError: ODFrameworkErrors

An invalid parameter was provided.

var kODErrorRecordPermissionError: ODFrameworkErrors

The changes were denied due to insufficient permissions.

var kODErrorRecordReadOnlyNode: ODFrameworkErrors

The record cannot be modified.

var kODErrorRecordTypeDisabled: ODFrameworkErrors

The record type is disabled by policy for a plug-in.

var kODErrorSessionDaemonNotRunning: ODFrameworkErrors

The daemon is not running.

var kODErrorSessionDaemonRefused: ODFrameworkErrors

The daemon refused the session.

var kODErrorSessionLocalOnlyDaemonInUse: ODFrameworkErrors

A normal request was issued when the local-only daemon was in use.

var kODErrorSessionNormalDaemonInUse: ODFrameworkErrors

A local-only request was issued when the normal daemon was in use.

var kODErrorSessionProxyCommunicationError: ODFrameworkErrors

There was a communication error with the remote daemon.

var kODErrorSessionProxyIPUnreachable: ODFrameworkErrors

The proxy did not respond.

var kODErrorSessionProxyUnknownHost: ODFrameworkErrors

The proxy could not be resolved.

var kODErrorSessionProxyVersionMismatch: ODFrameworkErrors

Versions mismatch between the remote daemon and the local framework.

var kODErrorSuccess: ODFrameworkErrors

var kODErrorCredentialsAccountLocked: ODFrameworkErrors

var kODErrorCredentialsAccountTemporarilyLocked: ODFrameworkErrors

var kODErrorCredentialsContactPrimary: ODFrameworkErrors

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

