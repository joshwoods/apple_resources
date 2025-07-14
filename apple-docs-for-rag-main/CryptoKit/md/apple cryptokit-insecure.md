

- Apple CryptoKit
-  Insecure 

Enumeration

# Insecure

A container for older, cryptographically insecure algorithms.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Insecure
```

## Overview

Important

These algorithms aren’t considered cryptographically secure, but the framework provides them for backward compatibility with older services that require them. For new services, avoid these algorithms.

## Topics

### Hashes

struct MD5

An implementation of MD5 hashing.

struct SHA1

An implementation of SHA1 hashing.

### Structures

struct MD5Digest

The output of a MD5 hash.

struct SHA1Digest

The output of a SHA1 hash.

## Relationships

### Conforms To

- Sendable

