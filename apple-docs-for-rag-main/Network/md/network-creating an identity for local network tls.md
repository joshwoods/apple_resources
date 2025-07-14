

- Network
-  Creating an Identity for Local Network TLS 

Article

# Creating an Identity for Local Network TLS

Learn how to create and use a digital identity in your application for local network TLS.

## Overview

In the context of Transport Layer Security (TLS), a *digital identity* is a cryptographic asset that contains a certificate and an associated private key for encrypting network traffic sent between a client and a server. Creating a digital identity for iOS or macOS is done so clients can communicate using TLS over the internet or a local network.

In this scenario, a server accepts client connections on a local network. While this article focuses on local network TLS, you can apply many of the concepts for other use cases. For example, setting up TLS with a certificate obtained from third-party Certificate Authority or configuring any system that needs to establish chain of trust to a root certificate.

### Prepare the Environment

Imagine you’re building an app to handle orders in a restaurant. This app runs on a server device — like an iPad or Mac — located at the front desk. Out in the restaurant, customers create and send orders to the server to be processed by the server using iOS client devices. In this situation, the server uses a digital identity from a local certificate authority to provide TLS to the clients. The following article explains how to setup both the server and client devices for local network TLS.

To create an identity for local network TLS the first thing you need to do is create and manage a local Certificate Authority (CA). A CA is a trusted entity that issues certificates for use in cryptographic operations. In this case, the CA serves as the trusted source of truth to issue a certificate that is used in a digital identity for TLS. Without this trusted authority, clients won’t be able to verify the issuer of the certificate they are using.

After creating the CA, you need to issue a leaf certificate for the digital identity that is installed on the server. Next, you need to distribute the identity to the server. In the restaurant example, this is either the macOS or iOS device acting as the server. Lastly, you also need to distribute the root certificate to all of the iOS client devices in the restaurant network so that they can establish the chain of trust during the handshake process, and trust evaluation doesn’t need to be overridden.

An overview of how this would work can be described as follows:

1.  Create and manage your own certificate authority using the Keychain app on macOS.

2.  Distribute the identity to the server. On macOS, either create and use an identity on the same machine the server is running on, or securely distribute the PKCS#12 file to the device Keychain. On iOS, import the PKCS#12 file onto the server device. For example, you could load the PKCS#12 file onto a thumb drive and import it to the iOS server app and save it in the Keychain.

3.  On iOS client devices, install the root certificate onto the iOS device to form the chain of trust.

### Distribute the Identity to the Server

On iOS, the certificate authority owner is faced with the challenge of distributing the identity to the server. After transferring the identity on the server — either through thumb drive or through secure network transfer — save it to the Keychain. To save the identity in the iOS Keychain, use the following:

```
```

To retrieve the identity from the iOS Keychain, use the following:

```
```

With the local identity accessible from the Keychain, set it to NWListener to serve connections using TLS 1.2+ with the following:

```
```

On macOS, the code is largely the same except if the `NWListener` is running on the same machine that set up the local certificate authority then the app’s code can reference the identity by loading a reference from the SecCertificate in the Keychain. To retrieve the identity from the Keychain on macOS, use the following:

```
```

After loading the identity on macOS, you can use the exact same `NWListener` code on iOS.

### Configure the Client Devices

For clients that connect to the server, install the root certificate on the client device to avoid overriding trust evaluation. After installing the root certificate on the client device, the client connects to the server using a local network name. When connecting from the client side of the connection, use the following:

```
```

Note

If the root certificate from the CA is installed on the device, you can use the code above without implementing sec_protocol_options_set_verify_block(_:_:_:) to override trust evaluation.

If your client needs to connect over IP, instead of using a local network name, the server needs to use a leaf certificate that lists the IP in the “IP Address” field of the Subject Alternative Name. This also avoids having to override trust evaluation on the client and allows client connections to use the following:

```
```

Attempting to connect from a client to a server without the root certificate installed on the client iOS device results in application errors similar to the following:

```
// [BoringSSL] boringssl_context_error_print(1863) boringssl ctx 0x2813acbe0: 4348594328:error:1000007d:SSL routines:OPENSSL_internal:CERTIFICATE_VERIFY_FAILED
// [BoringSSL] boringssl_session_handshake_incomplete(164) [C1:1][0x1032186d0] SSL library error
```

Note

The same is true if either the IP Address or DNS Name in the Subject Alternative Name fields are missing in the leaf certificate.

To work around this on the client, use `sec_protocol_options_set_verify_block` to perform your own verification checks on the peer’s leaf certificate. This isn’t the recommended path, but could be done in extreme cases. In the following example, SecPolicyCreateBasicX509() checks against the certificate’s basic x509 policy:

```
```

From there the client can set up a handshake using TLS on a local network.

## See Also

### Network Security and Privacy

Security Options

Configure security options for TLS handshakes.

Privacy Management

Configure parameters related to user privacy.

