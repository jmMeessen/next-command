# Next command

A handy tool to avoid typos during demonstrations.
It will load a command in the clipboard by reading a reference file one line at the time.

This tool is based on the demonstration made during the 2015 DEVOXX talk "60 useful Linux commands in 15 minutes" by Pierre-Antoine Grégoire (@zepag).

NOTE: the "pbcopy" utility used to copy the command to the clipboard works only on OSX. Replace it with an equivalent command for Linux.

## Usage

1. Create a file with the commands to be loaded
2. Export a variable with the name of that file with a command like `export command_list=my_filename`
3. Call recursively the `next-command.sh` script to load each line to the clipboard.
4. The loaded command can then be pasted with the usual `<cmd> v`

To restart the sequence, just delete the file with the extention `.wrk` 