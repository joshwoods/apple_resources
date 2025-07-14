

- Open Directory
-  OpenDirectory Constants 

API Collection

# OpenDirectory Constants

## Topics

### Constants

let ODFrameworkErrorDomain: String

let ODSessionProxyAddress: String

The address to connect to via proxy. The value is of type `NSString`.

let ODSessionProxyPassword: String

The password to connect with via proxy. The value is of type `NSString`.

let ODSessionProxyPort: String

The port to connect to via proxy. The value is of type `NSNumber`.

let ODSessionProxyUsername: String

The username to connect with via proxy. The value is of type `NSString`.

let ODTrustTypeAnonymous: String

let ODTrustTypeJoined: String

let ODTrustTypeUsingCredentials: String

let kODAttributeTypeAltSecurityIdentities: String

let kODAttributeTypeHardwareUUID: String

let kODAttributeTypeMetaAmbiguousName: String

let kODAttributeTypeMetaAugmentedAttributes: String

let kODAttributeTypeMetaRecordName: String

let kODAttributeTypeNodeOptions: String

let kODAttributeTypeNodeSASLRealm: String

let kODAttributeTypeOperatingSystem: String

let kODAttributeTypeOperatingSystemVersion: String

let kODAttributeTypeProfiles: String

let kODAttributeTypeProfilesTimestamp: String

let kODAttributeTypeTrustInformation: String

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

let kODErrorDomainFramework: CFString!

The error domain used for errors from the Open Directory framework.

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

let kODModuleConfigOptionConnectionIdleDisconnect: CFString!

let kODModuleConfigOptionConnectionSetupTimeout: CFString!

let kODModuleConfigOptionManInTheMiddle: CFString!

let kODModuleConfigOptionPacketEncryption: CFString!

let kODModuleConfigOptionPacketSigning: CFString!

let kODModuleConfigOptionQueryTimeout: CFString!

let kODNodeOptionsQuerySkippedSubnode: CFString!

let kODPolicyAttributeCreationTime: String

let kODPolicyAttributeCurrentDate: String

let kODPolicyAttributeCurrentDayOfWeek: String

let kODPolicyAttributeCurrentTime: String

let kODPolicyAttributeCurrentTimeOfDay: String

let kODPolicyAttributeDaysUntilExpiration: String

let kODPolicyAttributeEnableAtTimeOfDay: String

let kODPolicyAttributeEnableOnDate: String

let kODPolicyAttributeEnableOnDayOfWeek: String

let kODPolicyAttributeExpiresAtTimeOfDay: String

let kODPolicyAttributeExpiresEveryNDays: String

let kODPolicyAttributeExpiresOnDate: String

let kODPolicyAttributeExpiresOnDayOfWeek: String

let kODPolicyAttributeFailedAuthentications: String

let kODPolicyAttributeLastAuthenticationTime: String

let kODPolicyAttributeLastFailedAuthenticationTime: String

let kODPolicyAttributeLastPasswordChangeTime: String

let kODPolicyAttributeMaximumFailedAuthentications: String

let kODPolicyAttributeNewPasswordRequiredTime: String

let kODPolicyAttributePassword: String

let kODPolicyAttributePasswordHashes: String

let kODPolicyAttributePasswordHistory: String

let kODPolicyAttributePasswordHistoryDepth: String

let kODPolicyAttributeRecordName: String

let kODPolicyAttributeRecordType: String

let kODPolicyCategoryAuthentication: String

let kODPolicyCategoryPasswordChange: String

let kODPolicyCategoryPasswordContent: String

let kODPolicyKeyContent: String

let kODPolicyKeyContentDescription: String

let kODPolicyKeyEvaluationDetails: String

let kODPolicyKeyIdentifier: String

let kODPolicyKeyParameters: String

let kODPolicyKeyPolicySatisfied: String

let kODPolicyTypeAccountExpiresOnDate: String

let kODPolicyTypeAccountMaximumFailedLogins: String

let kODPolicyTypeAccountMaximumMinutesOfNonUse: String

let kODPolicyTypeAccountMaximumMinutesUntilDisabled: String

let kODPolicyTypeAccountMinutesUntilFailedLoginReset: String

let kODPolicyTypePasswordCannotBeAccountName: String

let kODPolicyTypePasswordChangeRequired: String

let kODPolicyTypePasswordHistory: String

let kODPolicyTypePasswordMaximumAgeInMinutes: String

let kODPolicyTypePasswordMaximumNumberOfCharacters: String

let kODPolicyTypePasswordMinimumNumberOfCharacters: String

let kODPolicyTypePasswordRequiresAlpha: String

let kODPolicyTypePasswordRequiresMixedCase: String

let kODPolicyTypePasswordRequiresNumeric: String

let kODPolicyTypePasswordRequiresSymbol: String

let kODPolicyTypePasswordSelfModification: String

let kODRecordTypeQueryInformation: String

let kODAuthenticationTypeClearTextReadOnly: String

let kODAuthenticationTypeMPPEPrimaryKeys: String

let kODBackOffSeconds: String

var kODErrorCredentialsAccountLocked: ODFrameworkErrors

var kODErrorCredentialsAccountTemporarilyLocked: ODFrameworkErrors

var kODErrorCredentialsContactPrimary: ODFrameworkErrors

## See Also

### Reference

OpenDirectory Functions

This document describes the functions, constants, and data types used to interact with Open Directory.

OpenDirectory Enumerations

OpenDirectory Data Types

