

- Endpoint Security
-  es_process_t 

Structure

# es_process_t

A type that describes a process, as delivered by an Endpoint Security message.

Mac CatalystmacOS

``` source
struct es_process_t
```

## Overview

For process events, this type also indicates the newly-executing process.

You can extract values such as the process identifier (`PID`), user identifier (`UID`), and group identifier (`GID`) from the audit_token field by using functions defined in `libbsm.h`.

### Working with Code Signing

Fields related to code signing, such as cdhash and signing_id, reflect the state of the process at the time Endpoint Security generated the message. In the specific case of process execution, this is after the `exec` completes in the kernel, but before any code in the process starts executing. At that point, XNU has validated the signature itself and has verified that the `cdhash` is correct. This second validation means that the hash of all individual page hashes in the Code Directory match the signed `cdhash`, essentially verifying the signature wasn’t tampered with. However, XNU doesn’t verify individual page hashes until the binary executes and pages in the corresponding pages. XNU doesn’t determine a binary shows signs of tampering until the individual pages page in, at which point XNU updates the code signing flags.

Endpoint Security provides clients the current state of the CS flags in the codesigning_flags member of the es_process_t structure. Keep the following points in mind when evaluating this field:

- The `CS_VALID` bit in codesigning_flags means that everything the kernel has validated up to that point in time was valid. However, this doesn’t mean there’s been a full validation of all the pages in the executable file. If a page’s content has been tampered with, XNU won’t know until that page pages in.

- When XNU detects a tampered page, it clears the `CS_VALID` bit. With the `CS_KILL` bit set, Endpoint Security terminates the process, preventing the tampered code from executing. Platform binaries and binaries that opted into the hardened runtime typically have the `CS_KILL` bit set.

- If you want your Endpoint Security client to detect tampered code before it pages in, such as at execution time, you can do so with the Security framework. However, this may impose a significant performance cost.

- Endpoint Security plays no role in verifying the validity of code signatures.

## Topics

### Inspecting the Source Process

var audit_token: audit_token_t

A token for use with Basic Security Module auditing functions.

var executable: UnsafeMutablePointer&lt;es_file_t>

The file containing the executed process.

var is_es_client: Bool

A Boolean value that indicates whether the process connects to the Endpoint Security subsystem.

var is_platform_binary: Bool

A Boolean value that indicates whether the process is a platform binary.

var start_time: timeval

The time the process started.

### Inspecting Process IDs

var ppid: pid_t

The parent process identifier.

var original_ppid: pid_t

The original parent process ID.

var group_id: pid_t

The process group identifier.

var session_id: pid_t

The identifier of the session that contains the process group.

var tty: UnsafeMutablePointer&lt;es_file_t>?

The TTY associated with the process sending the message.

### Inspecting Code Signing Properties

var codesigning_flags: UInt32

The flags used to sign the process.

var cdhash: es_cdhash_t

The code directory hash value.

var signing_id: es_string_token_t

The identifier used to sign the process.

var team_id: es_string_token_t

The team identifier used to sign the process.

### Inspecting Audit Tokens

var responsible_audit_token: audit_token_t

The audit token of the process responsible for this process.

var parent_audit_token: audit_token_t

The audit token of the parent process.

### Initializers

init(audit_token: audit_token_t, ppid: pid_t, original_ppid: pid_t, group_id: pid_t, session_id: pid_t, codesigning_flags: UInt32, is_platform_binary: Bool, is_es_client: Bool, cdhash: es_cdhash_t, signing_id: es_string_token_t, team_id: es_string_token_t, executable: UnsafeMutablePointer&lt;es_file_t>, tty: UnsafeMutablePointer&lt;es_file_t>?, start_time: timeval, responsible_audit_token: audit_token_t, parent_audit_token: audit_token_t)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Inspecting Event Properties

var target: UnsafeMutablePointer&lt;es_process_t>

The process to execute.

