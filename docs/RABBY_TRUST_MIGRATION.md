# Rabby Trust Migration Baseline

- **Original Commit**: `56c05ddaa build: prepare publish 0.6.91 (#2199)`
- **Branch**: `develop`
- **Backup Branch**: `backup/pre-rabby-trust`
- **Backup Tag**: `pre-rabby-trust-baseline`
- **Migration Date**: 2026-09-29
- **Target Brand**: Rabby Trust
- **Bundle ID**: `com.rabbytrust.wallet` (Debug: `com.rabbytrust.wallet.debug`)
- **Key Changes**:
  - Independent Apple identity and neutral bundle IDs
  - Removal of DeBank Apple Developer Team ID (`ZPNP2SF27Q`)
  - Cleanup of dead permissions (`NSMicrophoneUsageDescription`) and SiriKit call/message intents
  - Rebranding display name and user-facing copy to Rabby Trust
  - Neutralizing foreign Sentry / Firebase / WalletConnect project bindings
  - Release APNs configuration set to production
- **External Dependencies / Blockers**:
  - Requires user Apple Developer Team selection in Xcode
  - User WalletConnect / Reown Cloud Project ID placeholder
  - External Rabby OpenAPI backend dependency documented
