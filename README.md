# lua-resty-murmurhash2

`lua-resty-murmurhash2` is MurmurHash 2 library (LuaJIT bindings) for OpenResty's / Nginx's murmurhash2 implementation.

## Installation

Just place [`murmurhash2.lua`](https://github.com/bungle/lua-resty-murmurhash2/blob/master/lib/resty/murmurhash2.lua) somewhere in your `package.path`, preferably under `resty` directory. If you are using OpenResty, the default location would be `/usr/local/openresty/lualib/resty`.

### Using LuaRocks or MoonRocks

If you are using LuaRocks >= 2.2:

```Shell
$ luarocks install lua-resty-murmurhash2
```

If you are using LuaRocks < 2.2:

```Shell
$ luarocks install --server=http://rocks.moonscript.org moonrocks
$ moonrocks install lua-resty-murmurhash2
```

MoonRocks repository for `lua-resty-murmurhash2`  is located here: https://rocks.moonscript.org/modules/bungle/lua-resty-murmurhash2.

## Lua API
#### number require "resty.murmurhash2" string

This module has only one function that you can get just by requiring this module:

```lua
local mmh2 = require "resty.murmurhash2"
local hash = mmh2 "test" -- hash contains number 403862830
```

## License

`lua-resty-session` uses two clause BSD license.

```
Copyright (c) 2014, Aapo Talvensaari
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

* Redistributions of source code must retain the above copyright notice, this
  list of conditions and the following disclaimer.

* Redistributions in binary form must reproduce the above copyright notice, this
  list of conditions and the following disclaimer in the documentation and/or
  other materials provided with the distribution.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
```
