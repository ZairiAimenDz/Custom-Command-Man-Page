# Creating MAN Pages

## Where to Put

Look For It In One Of These Folders :

MANPATH /usr/man

MANPATH /usr/share/man

MANPATH /usr/local/man

MANPATH /usr/local/share/man

MANPATH /usr/X11R6/man

Inside That Choose man1 to 9 depending on your custom command type (These Are Just Some Usual Ones):

1 - > Executable Commands

2 - > System Calls

6 - > Games

7 - > Miscellaneous

The File Is with an extension of the number of the type like ls.1 and var.2 etc
## How To Make

This Is The Basic Syntax For Every Menu Page :

.\" Manpage for (Your Custom Commands)
.\" Extra Stuff That You Can Put Here Like Your Email And Stuff.
.TH man 1 "8 Dec 2019" "0.1" "(Your Custom Command) man page"
.SH NAME
(Custom Command Name) \- What It Does.
.SH SYNOPSIS
(Syntax to get your command working) like man [command].
.SH DESCRIPTION
a description of your custom command.
.SH OPTIONS
the options like -l in ls and etc.
.SH SEE ALSO
useradd(8), passwd(5), nuseradd.debian(8) (Extra Commands ToCheck)
.SH BUGS
No known bugs.
.SH AUTHOR
You

## How To Use

The Name Of The File Is the name you use with the man command
