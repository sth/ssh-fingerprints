# ssh-fingerprints

Show fingerprints of all ssh host keys as MD5 and SHA256, even if ssh-keygen
doesn't support the `-E` option.

## Motivation

When connecting to a server from a new machine, ssh usually prompts you with
the fingerprint of the server. Since there are several fingerprint algorithms
and usually several keys, it can be inconvenient to find the correct server
fingerprint. Additionally, older versions of `ssh-keygen` don't support the `-E`
option to select the fingerprint algorithm, further complicating things.

This script shows the fingerprints of all keys in both MD5 and SHA256 formats.

## Dependencies

Requires `bash`, `openssl` and `base64`
