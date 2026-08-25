# mikicaChessEngine releases

This public repository contains official prebuilt binaries of
**mikicaChessEngine**. The development repository and source history remain
private; no source code is published here.

## Latest stable release

Download [`v0.3.0`](https://github.com/oaki/mikicaChessEngine-releases/releases/tag/v0.3.0).

Available packages:

- Linux x86-64 generic — compatibility default
- Linux x86-64 Haswell/AVX2
- Windows x86-64 generic — compatibility default
- Windows x86-64 Haswell/AVX2

Use a generic package unless the target CPU is known to support the Haswell
instruction set. Recommended tournament configuration is `Threads=1`,
`Hash=256`, pondering off, with an externally supplied common opening book.

## Verify a download

Linux or macOS:

```sh
shasum -a 256 -c SHA256SUMS.txt
```

Windows PowerShell:

```powershell
Get-FileHash .\mikicaChessEngine-v0.3.0-windows-x86_64-generic.zip -Algorithm SHA256
```

Compare the result with the corresponding line in `SHA256SUMS.txt`.

## Scope

The current stable release is a single-thread UCI engine. It does not claim
Stockfish parity, an official CCRL rating, multi-thread strength, NNUE, or
engine-side Syzygy support.

Binary releases are produced and UCI-smoke-tested on native Linux and Windows
GitHub-hosted runners in the private development repository. Only the verified
archives, checksums, and release notes are copied here automatically.
