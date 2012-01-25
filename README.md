# multiple-cursors.el

An experiment in multiple cursors for emacs. Still very much in beta.

The basic concept works, but there are definitely some kinks to work out.

This extension is dependent on the mark-multiple library.

    https://github.com/magnars/mark-multiple.el

## Usage

I've set up my key-bindings like so:

    ;; Experimental multiple-cursors
    (global-set-key (kbd "C-S-c C-S-c") 'mc/add-multiple-cursors-to-region-lines)
    (global-set-key (kbd "C-S-c C-e") 'mc/edit-ends-of-lines)
    (global-set-key (kbd "C-S-c C-a") 'mc/edit-beginnings-of-lines)

To get out of multiple-cursors-mode, press `C-g`.

You can also switch to multiple-cursors-mode by pressing C-g when in
mark-multiple-mode. This is symmetrical to how pressing C-g with an active
region deactivates it. Press C-g again to remove extra cursors.

## Contribute

There's plenty wrong with this implementation still. I'm actively trying things
out, and also considering combining it with
[mark-multiple.el](https://github.com/magnars/mark-multiple.el) to get a more
comprehensive tool.

Still, if you've got something to contribute, please do not hesitate to open
an issue, and we can take a look together before you dive into the elisp. :-)

You'll find the repo at:

    https://github.com/magnars/multiple-cursors.el

## License

Copyright (C) 2011 Magnar Sveen

Author: Magnar Sveen <magnars@gmail.com>
Keywords: editing cursors

This program is free software; you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
