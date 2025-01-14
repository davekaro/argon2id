# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.2] - 2024-11-01

### Fixed

- Validate that the encoded hash passed to Argon2id::Password.new is a
  null-terminated C string, raising an ArgumentError if it contains extra null
  bytes

## [0.1.1] - 2024-11-01

### Added

- RDoc documentation for the API

### Fixed

- Saved a superfluous extra byte when allocating the buffer for the encoded
  hash

## [0.1.0] - 2024-10-31

### Added

- The initial version of the Argon2id gem, providing Ruby bindings to the
  reference C implementation of Argon2, the password-hashing function that won
  the Password Hashing Competition.

[0.1.2]: https://github.com/mudge/argon2id/releases/tag/v0.1.2
[0.1.1]: https://github.com/mudge/argon2id/releases/tag/v0.1.1
[0.1.0]: https://github.com/mudge/argon2id/releases/tag/v0.1.0
