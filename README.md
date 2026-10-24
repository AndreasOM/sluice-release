# sluice

sluice: my take on driving external controllers such as Stream Decks. Client/server, multi-client, cross-platform, extendable.

Binaries: [Releases](../../releases), one tarball per platform.

## Changelog

- 0.2.0 (2026-10-23): first pre-release, macOS arm64 only.

## License

MIT OR Apache-2.0, see `LICENSE-MIT` and `LICENSE-APACHE`.

## Plugins confirmed working

One row per plugin someone ran on real hardware or in CI; "untested" is not "broken". Columns are the release targets. The release workflow copies this table into the public release README.

| Plugin | Kind | macOS arm64 | Linux x86_64 | Windows x86_64 | Notes |
|---|---|---|---|---|---|
| Elgato CPU (`com.elgato.cpu`) | vendor `*.sdPlugin` via `sluice-plugin-sdhost` | yes, Neo, 2026-10-22 | untested | untested | installed by the vendor app; quit the app first |
| TikClock (`com.gdwhisper.tikclock` 1.1.0) | OpenAction, native | yes, Neo, 2026-10-22; property inspector in the browser 2026-10-24 | yes, CI on a dummy Neo | untested | pinned download in `scripts/openaction-smoke.sh` |
| `sluice-plugin-ram` | sluice native provider (in the tarball) | yes, Neo, 2026-10-23 | yes, CI | untested | |
| `sluice-plugin-echo` | sluice native (in the tarball) | yes | yes, CI | untested | smallest plugin, logs invocations |
