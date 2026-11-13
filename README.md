# claude-mods

Mods for Claude Code.

## session-band-zones

A band above the prompt with the session at a glance: smart/dumb zone by context size, turn number, output speed, cost, and a countdown for the prompt cache. See [session-band-zones/README.md](session-band-zones/README.md) for details.

**Credit:** this is a modified version of the `session-band` mod by [johnnyvizz](https://github.com/johnnyvizz), from his [claude-kit](https://github.com/johnnyvizz/claude-kit) repository (MIT). The band, cache countdown and notifier are his work. The addition here is the smart-zone / dumb-zone indicator. His license and copyright notice are in [LICENSE](LICENSE). If you want the original, unmodified mod, or his other mods and skills, install them from his repository instead:

```
/plugin marketplace add johnnyvizz/claude-kit
/plugin install session-band@claude-kit
```

This version is not maintained by him. Please don't send him bug reports about the zone indicator.

### Install

At the prompt of a terminal Claude Code session:

```
/plugin install session-band-zones --marketplace shannonc525/claude-mods
```

Answer `y` to add the marketplace, then pick a scope (user scope loads it in every session).

From a shell:

```
claude plugin install session-band-zones --marketplace shannonc525/claude-mods
```

In the desktop app, where `/plugin` does not run: click + next to the prompt box, then Plugins, Add marketplace with `shannonc525/claude-mods`, then Add plugin.

### Optional: macOS notifier

For the cache-expiry notification with a title and click-through, build the helper app once (needs Xcode's command line tools). Find the installed mod's folder with `claude plugin list`, then run `notifier/build.sh` there.
