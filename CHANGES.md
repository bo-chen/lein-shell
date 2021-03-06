# lein-shell changelog

## 0.5.0 [`tag`][0.5.0-tag]

* Fixed a bug where non-string were not converted to strings before sent to the
  command, causing NullPointerExceptions, cast errors and other problems.
* Implemented parameter expansion. You can specify them on the form `${:foo}`
  and on the form `${[:foo :bar]}`. They can also contain default strings.

## 0.4.2 [`tag`][0.4.2-tag]

* Fixed a bug where lein-shell itself could not be used as a higher order alias
  in certain scenarios.

## 0.4.1 [`tag`][0.4.1-tag]

* Custom `:shell :commands` can now be vectors instead of strings only, acting
  more or less like Lein aliases.

## 0.4.0 [`tag`][0.4.0-tag]

* By default, stdin is piped in to shell commands. You can now specify that
  lein-shell doesn't pipe stdin to the shell command.
* A `:default-command` option can be specified as a catch-all for os-specific
  commands, which can be used to create aliases.

## 0.3.0 [`tag`][0.3.0-tag]

* Exit-code handling, directory specification and environment settings can now
  be set on a per-command basis.
* It is now possible to ignore exit codes from commands, if wanted.
* Fixed a bug where reading from Stdin resulted in only partial input
  redirection.

## 0.2.0 [`tag`][0.2.0-tag]

* Fixed a bug where the exit-code of a process was ignored.
* It is now possible to specify a directory in which to start commands. This is
  by default the root folder of a project.
* Added possibility to add/replace environment variable settings.
* Implemented functionality to specify aliases for commands based on which
  operative system you are using.

## 0.1.0 [`tag`][0.1.0-tag]

* First release!

[0.5.0-tag]: https://github.com/hyPiRion/lein-shell/tree/0.5.0
[0.4.2-tag]: https://github.com/hyPiRion/lein-shell/tree/0.4.2
[0.4.1-tag]: https://github.com/hyPiRion/lein-shell/tree/0.4.1
[0.4.0-tag]: https://github.com/hyPiRion/lein-shell/tree/0.4.0
[0.3.0-tag]: https://github.com/hyPiRion/lein-shell/tree/0.3.0
[0.2.0-tag]: https://github.com/hyPiRion/lein-shell/tree/0.2.0
[0.1.0-tag]: https://github.com/hyPiRion/lein-shell/tree/0.1.0

