# Ferrum

> Theme and plugin loader for Discord's upcoming native Rust desktop client. Think Vencord, but for the post-Electron app.

**Status: early research. Nothing works yet. There is no download.**

## Why

Discord is replacing its Electron desktop app with a native client written in Rust (built on [GPUI](https://www.gpui.rs/)). Once that ships, CSS themes and JavaScript mods like Vencord and BetterDiscord will stop working, because there is no web page left to inject into.

Ferrum aims to bring themes and plugins back to the native client.

## Planned approach

- **Loader:** a small Rust DLL loaded alongside the Discord client
- **Hooks:** signature scanning and function hooking, so updates break as little as possible
- **Themes:** color themes from simple JSON files
- **Installer:** one click to install, uninstall, and re-apply after Discord updates
- **Plugins (later):** a scripting API on top of the hooks

## Roadmap

- [ ] Research GPUI internals using open-source GPUI apps (e.g. Zed)
- [ ] Proof of concept: re-theme a GPUI app at runtime
- [ ] Analyze the Discord native client once a public build exists
- [ ] Loader + color themes
- [ ] Installer
- [ ] Plugin API

## Related

- [discord-themes-fixed](https://github.com/KAZRUTx/discord-themes-fixed): old BetterDiscord themes fixed for the current (Electron) Discord

## Disclaimer

Ferrum is not affiliated with or endorsed by Discord Inc. Client modifications are against Discord's Terms of Service and may get your account banned. Use at your own risk.

## License

GPL-3.0
