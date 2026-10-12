# Equipment Maintenance Decision System — Public Releases

This public repository contains only verified, portable installation archives
and SHA-256 checksums. The application source repository remains private.

## Current release: poc-v2.16.47

[Download poc-v2.16.47](https://github.com/dddabtc/equip-maint-ai-releases/releases/tag/poc-v2.16.47)
— includes the database backup reliability fixes for
[issue #1](https://github.com/dddabtc/equip-maint-ai-releases/issues/1).
Failed automatic backups now respect the configured interval, release SQLite
handles, clean up owned temporary files, and check available disk space.
After five consecutive failures, fix the cause and complete one manual backup
to resume automatic backups.

Before upgrading, stop the old application and preserve your existing runtime
data, configuration, and backups. Do not overwrite site data with demonstration
data. Native Windows tests are not a field certification for Windows Server 2016
or third-party antivirus compatibility.

Download the archive matching your operating system and CPU architecture from
the **Releases** page. Each archive is self-contained: unpack it into a writable
directory and run the included launcher. No Python or dependency installation
is required.

## Available platforms

- Windows x64
- Windows ARM64
- macOS x64 (Intel)
- macOS ARM64 (Apple silicon)
- Linux x64
- Linux ARM64

Verify the downloaded archive with its adjacent `.sha256` file or the combined
`SHA256SUMS.txt` before running it.

The included demonstration knowledge and cases are fictional and contain no
customer-identifying information. They are intended for product evaluation,
not as a substitute for site procedures, equipment manuals, or safety rules.
