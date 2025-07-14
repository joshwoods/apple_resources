

- Security
-  SecProtocolType 

Enumeration

# SecProtocolType

The protocol type associated with an Internet password.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecProtocolType
```

## Topics

### Constants

case FTP

Indicates FTP.

case ftpAccount

Indicates a client side FTP account. The usage of this constant is deprecated as of macOS 10.3.

case HTTP

Indicates HTTP.

case IRC

Indicates IRC.

case NNTP

Indicates NNTP.

case POP3

Indicates POP3.

case SMTP

Indicates SMTP.

case SOCKS

Indicates SOCKS.

case IMAP

Indicates IMAP.

case LDAP

Indicates LDAP.

case appleTalk

Indicates AFP over AppleTalk.

case AFP

Indicates AFP over TCP.

case telnet

Indicates Telnet.

case SSH

Indicates SSH.

case FTPS

Indicates FTP over TLS/SSL.

case HTTPS

Indicates HTTP over TLS/SSL.

case httpProxy

Indicates HTTP proxy.

case httpsProxy

Indicates HTTPS proxy.

case ftpProxy

Indicates FTP proxy.

case CIFS

Indicates CIFS.

case SMB

Indicates SMB.

case RTSP

Indicates RTSP.

case rtspProxy

Indicates RTSP proxy.

case DAAP

Indicates DAAP.

case EPPC

Indicates Remote Apple Events.

case IPP

Indicates IPP.

case NNTPS

Indicates NNTP over TLS/SSL.

case LDAPS

Indicates LDAP over TLS/SSL.

case telnetS

Indicates Telnet over TLS/SSL.

case IMAPS

Indicates IMAP4 over TLS/SSL.

case IRCS

Indicates IRC over TLS/SSL.

case POP3S

Indicates POP3 over TLS/SSL.

case cvSpserver

Indicates CVS pserver.

case SVN

Indicates Subversion.

case any

Indicates that any protocol is acceptable.

### Initializers

init?(rawValue: FourCharCode)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

