# NAME

mdnumr - A Perl script to add numbering to markdown headers and manage backup files

# VERSION

0.0.2 (2024.10.01.)

# SYNOPSIS

**mdnumr** is a script that adds numbering to markdown file headers and optionally creates backup files.

Usage:

    mdnumr [options] file1.md file2.md ...

Options:

    -r, --range       Specify the range of header levels to number. Default is '1-6'.
    -z, --set-zero    Start numbering from zero.
    -b, --backup      Enable backup of original files with a '.bak' extension.
    -v, --version     Show the script version.
    -h, --help        Display help information.
    -m, --man         Display the manual page.

# DESCRIPTION

**mdnumr** is designed to automatically add numeric prefixes to headers in markdown files, making it easier to organize and reference sections. The script processes each file provided as an argument, adding numbers to headers within the specified range (e.g., h1 to h6 headers).

If the **--backup** option is enabled, a backup of each processed file is created with a '.bak' extension. The script also ensures that the numeric prefixes do not interfere with existing content by carefully managing the numbering and avoiding modification of code blocks.

Additionally, the script appends a comment marker to the end of each file to prevent re-processing of files that have already been numbered.

# LICENSE

This project is licensed under the GNU General Public License v3.0
