<!-- markdownlint-disable -->
<div align="center">
    <br />
    <h3>@visoftware/discord-rpc</h3>
    <br />
    <p>
        <a href="https://www.npmjs.com/package/@visoftware/discord-rpc" target="_blank"><img src="https://img.shields.io/npm/v/@visoftware/discord-rpc.svg" alt="npm version"/></a>
    </p>
</div>
<!-- markdownlint-enable -->

## About

`@vi-software/discord-rpc` is a fork of [@xmcl/discord-rpc](https://github.com/xmcl/discord-rpc) for [VI Software Launcher](https://github.com/VI-Software/vis-launcher/) with type safety and some additional features.

## Example

```ts
import { Client } from "@visoftware/discord-rpc";

const client = new Client({
    clientId: "123456789012345678"
});

client.on("ready", () => {
    client.user?.setActivity({
        state: "Hello, world!"
    });
});

client.login();
```

## Credits

- [discordjs](https://github.com/discordjs): Making [discordjs/RPC](https://github.com/discordjs/RPC)
- [@xmcl](https://github.com/xmcl): Original fork [@xmcl/discord-rpc](https://github.com/xmcl/discord-rpc)
- [@xhayper](https://github.com/xhayper): Fork [@xhayper/discord-rpc](https://github.com/xhayper/discord-rpc) that this is based on
- [JakeMakesStuff](https://github.com/JakeMakesStuff): [snap support](https://github.com/discordjs/RPC/pull/152)
- [Snazzah](https://github.com/Snazzah): [snap + flatpak support](https://github.com/Snazzah/SublimeDiscordRP/blob/c13e60cdbc5de8147881bb232f2339722c2b46b4/discord_ipc/__init__.py#L208)
- [leonardssh](https://github.com/leonardssh): Making [coc-discord-rpc](https://github.com/leonardssh/coc-discord-rpc) which inspried to make this package due to how old [discordjs/RPC](https://github.com/discordjs/RPC) is
