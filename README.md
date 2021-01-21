# Creating MAN Pages

## Where to Put

You Can Put It Inside One Of These Folders:
```

MANPATH /usr/man

MANPATH /usr/share/man

MANPATH /usr/local/man

MANPATH /usr/local/share/man

MANPATH /usr/X11R6/man

```

Inside That Choose man1 to 9 depending on your custom command type (These Are Just Some Usual Ones):

1 - > Executable Commands

2 - > System Calls

6 - > Games

7 - > Miscellaneous

The Command Man Page File Should Have An Extension Of The Same Number As The Folder It is in, like ls.1 is in folder 1 and var.2 is in folder 2 ... etc

The Command Man Page File Should Have The Same Name As Your Command So If You Name It Test you call it by doing 
`````
~$ man Test
`````
## How To Make

This Is The Basic Syntax For Every Menu Page (Remove The Brackets => []):
````

.\" Manpage for [THe Name Of Your Command]

.\" [You Can Put Subtitles or Your Email Or Any Extra Thing You Have]

.TH man 1 "8 Dec 2019" "0.1" "[Commmand Name] man page"

.SH NAME

[Command Name] \- [What It Does].

.SH SYNOPSIS

[Syntax To Use Your Command For Example : max [Command Name], ls [Folder] and so on]

.SH DESCRIPTION

[a description of your custom command].

.SH OPTIONS

[the options like -l in ls, -r in rm and more].

.SH SEE ALSO

useradd(8), passwd(5), nuseradd.debian(8) [Extra Commands ToCheck]

.SH BUGS

[Write If There Are Bugs That Have To Be Fixed]

.SH AUTHOR

[Your Name, COmpany Name, Team Name ..... Or Whatever ]
``````

And That's It, It's very easy To Do And If You are A linux user and want to automate some of your workflows creating a custom command with it's respective man page is the best way to do it.

