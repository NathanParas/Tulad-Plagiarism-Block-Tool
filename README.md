# Tulad #

Tulad is a plugin created for Moodle meant to detect cheating in forum posts. This version of Tulad is a block plugin that fetches all forum data and displays them inside a block. Additional buttons are displayed besides the forum posts that will generate two similarity indexes based on lexical and semantic standards relative to other forum posts. The similarity index for the lexical standard utilizes the Sorensen-Dice Coefficient and the semantic standard utilizes cosine similarity with Term Frequency - Inverse Document Frequency. A high similarity index might indicate traces of cheating. Please note of the keyword 'might' since both implementations are both crude and will not necessarily be always accurate.


## Installing via uploaded ZIP file ##

1. Log in to your Moodle site as an admin and go to _Site administration >
   Plugins > Install plugins_.
2. Upload the ZIP file with the plugin code. You should only be prompted to add
   extra details if your plugin type is not automatically detected.
3. Check the plugin validation report and finish the installation.

## Installing manually ##

The plugin can be also installed by putting the contents of this directory to

    {your/moodle/dirroot}/blocks/tulad

Afterwards, log in to your Moodle site as an admin and go to _Site administration >
Notifications_ to complete the installation.

Alternatively, you can run

    $ php admin/cli/upgrade.php

to complete the installation from the command line.

## License ##

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see <https://www.gnu.org/licenses/>.

