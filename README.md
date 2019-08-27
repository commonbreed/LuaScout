# LuaScout
<p align="center"><img src="lua_scout.png" alt="LuaScout Logo" width="200"/><br />
  A command-line tool for finding <a href="https://www.lua.org/">Lua</a> interpreters embedded within binaries.</p>

## Project rationale
This project was started to address a personal need to identify and interact with embedded Lua interpreters. Many applications use Lua as an internal scripting engine, to ease development and encourage extensibility. LuaScout facilitates (static) function pointer identification from signatures generated from any given Lua release, generating a portable C-code output capable of attaching hooks to these functions during runtime (a library injection tool is required - not provided here). Using compile-time options, this code can either dump a trace of calls to Lua functions, or act as a "man-in-the-middle" to hijack and modify Lua calls. Thanks to the architecture of the Lua language, this is actually rather simple. :)

### Nomenclature guidelines

| Object Type | Guideline                                           |
| ----------- | -----------------------------------------------     |
| Directory   | **lowercase**, no whitespace, no hyphenation        |
| File        | **CapitalCamelCase**, no whitespace, no hyphenation |
| Class       | **CapitalCamelCase**, no whitespace, no hyphenation |
| Local var   | **camelCase**, no whitespace, no hyphenation        |

  
