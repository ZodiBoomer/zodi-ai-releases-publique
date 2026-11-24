# Zodi AI — Public Releases

This repository distributes **downloadable application binaries and update metadata only**.

- Windows: signed/unsigned installer `.exe` (depending on release pipeline configuration).
- Android: signed `.apk`.
- Linux: `.deb` and portable `.tar.gz`.
- Update metadata: `latest.json`.

The application source code remains in private repositories:
- `ZodiBoomer/zodi-ai`
- `ZodiBoomer/zodi-ai-android`

## Download

See [GitHub Releases](https://github.com/ZodiBoomer/zodi-ai-releases-publique/releases/latest).

## Security and integrity

- Never upload source code, API keys, access tokens, signing keystores, passwords, private configuration, or user data here.
- Release assets must come from successful CI builds.
- Android APKs must be signed with the stable release key; do not distribute debug APKs as production updates.
- Each release should include a versioned tag and SHA-256 checksums.
- The update manifest is informational metadata, not a substitute for signature verification.

## Update manifest

`latest.json` is updated by trusted CI after successful publication. Clients should validate HTTPS, version compatibility, checksums, and platform architecture before installing an update.
