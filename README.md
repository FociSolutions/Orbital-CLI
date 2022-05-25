# orbital-cli

A command-line interface to manage the [Orbital Mock Server](https://orbitalmock.com).

<!-- toc -->

- [orbital-cli](#orbital-cli)
- [Usage](#usage)
- [Commands](#commands)
<!-- tocstop -->

# Usage

<!-- usage -->

```sh-session
$ npm install -g orbital-cli
$ orbital COMMAND
running command...
$ orbital (--version)
orbital-cli/0.1.0 darwin-x64 node-v16.14.2
$ orbital --help [COMMAND]
USAGE
  $ orbital COMMAND
...
```

<!-- usagestop -->

# Commands

<!-- commands -->

- [`orbital help [COMMAND]`](#orbital-help-command)
- [`orbital plugins`](#orbital-plugins)
- [`orbital plugins:install PLUGIN...`](#orbital-pluginsinstall-plugin)
- [`orbital plugins:inspect PLUGIN...`](#orbital-pluginsinspect-plugin)
- [`orbital plugins:install PLUGIN...`](#orbital-pluginsinstall-plugin-1)
- [`orbital plugins:link PLUGIN`](#orbital-pluginslink-plugin)
- [`orbital plugins:uninstall PLUGIN...`](#orbital-pluginsuninstall-plugin)
- [`orbital plugins:uninstall PLUGIN...`](#orbital-pluginsuninstall-plugin-1)
- [`orbital plugins:uninstall PLUGIN...`](#orbital-pluginsuninstall-plugin-2)
- [`orbital plugins update`](#orbital-plugins-update)

## `orbital help [COMMAND]`

Display help for orbital.

```
USAGE
  $ orbital help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for orbital.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.12/src/commands/help.ts)_

## `orbital plugins`

List installed plugins.

```
USAGE
  $ orbital plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ orbital plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.1.0/src/commands/plugins/index.ts)_

## `orbital plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ orbital plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ orbital plugins add

EXAMPLES
  $ orbital plugins:install myplugin

  $ orbital plugins:install https://github.com/someuser/someplugin

  $ orbital plugins:install someuser/someplugin
```

## `orbital plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ orbital plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ orbital plugins:inspect myplugin
```

## `orbital plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ orbital plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ orbital plugins add

EXAMPLES
  $ orbital plugins:install myplugin

  $ orbital plugins:install https://github.com/someuser/someplugin

  $ orbital plugins:install someuser/someplugin
```

## `orbital plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ orbital plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ orbital plugins:link myplugin
```

## `orbital plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ orbital plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ orbital plugins unlink
  $ orbital plugins remove
```

## `orbital plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ orbital plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ orbital plugins unlink
  $ orbital plugins remove
```

## `orbital plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ orbital plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ orbital plugins unlink
  $ orbital plugins remove
```

## `orbital plugins update`

Update installed plugins.

```
USAGE
  $ orbital plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

<!-- commandsstop -->
