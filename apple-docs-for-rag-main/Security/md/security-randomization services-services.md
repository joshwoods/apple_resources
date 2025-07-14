

- Security
-  Randomization Services 

API Collection

# Randomization Services

Generate cryptographically secure random numbers.

## Overview

Many security operations rely on randomization to avoid reproducibility. This is true for many complex cryptographic operations, such as key generation, but is also true for something as simple as generating a password string that can’t be easily guessed. If the string’s characters are truly random (and kept hidden), an attacker has no choice but to try every possible combination one at a time in a brute force attack. For sufficiently long strings, this becomes unfeasible.

But the strength of such a password depends on the quality of the randomization. True randomization is not possible in a deterministic system, such as one where software instructions from a bounded set are executed according to well-defined rules. But even “good” randomization (in a statistical sense) is difficult to produce under these conditions. If an attacker can infer patterns in insufficiently randomized data, your system becomes compromised. Use randomization services to generate a cryptographically secure set of random numbers.

## Topics

### Random Numbers

func SecRandomCopyBytes(SecRandomRef?, Int, UnsafeMutableRawPointer) -> Int32

Generates an array of cryptographically secure random bytes.

typealias SecRandomRef

An abstract Core Foundation-type object containing information about a random number generator.

let kSecRandomDefault: SecRandomRef

An alias for the default random number generator.

