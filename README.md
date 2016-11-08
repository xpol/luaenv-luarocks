# luaenv-luarocks

luaenv-luarocks is an [luaenv][] plugin that provides a `luaenv luarocks` command to configure and install LuaRocks on UNIX-like systems (where luaenv installs).

## Installation

Before using luaenv-luarocks, you need to install [luaenv][] and Lua with [lua-build][].

Installing luaenv-luarocks as an luaenv plugin will give you access to the `luaenv luarocks` command.

```shell
git clone https://github.com/xpol/luaenv-luarocks.git ~/.luaenv/plugins/luaenv-luarocks
```

This will install the latest development version of luaenv-luarocks into the `~/.luaenv/plugins/luaenv-luarocks` directory.
To update luaenv-luarocks, run `git pull` in `~/.luaenv/plugins/luaenv-luarocks` to download the latest changes.

[luaenv]: https://github.com/cehoffman/luaenv
[lua-build]: https://github.com/cehoffman/lua-build


## Usage

To install a LuaRocks for the current Lua in luaenv, run `luaenv luarocks` with the exact name of the version you want to install. For example,

```shell
luaenv luarocks 2.4.1
```

If no version name specified, the latest known stable release will used.

LuaRocks versions will be installed for current Lua in luaenv.

To see a list of all available LuaRocks versions, run `luaenv luarocks --list`.
