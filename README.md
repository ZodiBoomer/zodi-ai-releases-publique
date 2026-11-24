# Zodi AI — Public Releases

This repository distributes **downloadable application binaries and update metadata only**.

- Windows: installer `.exe`.
- Android: signed `.apk`.
- Linux: `.deb` and portable `.tar.gz`.
- Release-specific metadata: `latest-desktop.json` and `latest-android.json` attached to each GitHub Release.

The application source code remains in private repositories:
- `ZodiBoomer/zodi-ai`
- `ZodiBoomer/zodi-ai-android`

## Download

See [GitHub Releases](https://github.com/ZodiBoomer/zodi-ai-releases-publique/releases).

## Security and integrity

- Never upload source code, API keys, access tokens, signing keystores, passwords, private configuration, or user data here.
- Release assets must come from successful CI builds.
- Android APKs must be signed with the stable release key; debug APKs are never production updates.
- Releases must include SHA-256 checksums and versioned tags.
- Release metadata is informational; clients must verify checksums and platform compatibility before installing.

## Update metadata

The root `latest.json` is a schema placeholder. CI attaches platform-specific metadata to each release:
- `latest-desktop.json`
- `latest-android.json`

Clients should query the latest compatible release over HTTPS, validate version compatibility, verify SHA-256, and require system confirmation before installing.
