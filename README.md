vim-templ
=========

This is an extremely simple templating plugin for Vim since none of the
existing ones seemed to meet my needs.

Currently it's likely that this plugin isn't of much use to anybody else, but
for the record you can create templates in the `~/.vim/templates` directory
(not currently configurable) which are simple plain text files. These can then
be inserted into the current document with `:LoadTemplate <name>` where
`<name>` is the filename of the template. This command will tab-complete names
of templates.

There are currently two tokens which will be replaced during the substitution:

* '{UUID}' will be replaced by a random UUID (requires `uuidgen` utility).
* '{DT:x}' will be replaced by the current date/time where `x` is a
  `strftime()` format.

In the event that anybody does find this plugin useful and wants to request
some changes, by all means drop me a line at andy@andy-pearce.com.

