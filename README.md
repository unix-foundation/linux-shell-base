
<br>
<div align='center'>
  <img src='/../images/logo-light.png' width='37.2%' alt='logo-light.png'>
</div>
<br>
<br>

<p align='center'>
  <a href='https://github.com/linux-shell-base/packaged-utilities'>Packaged utilities</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href='https://github.com/linux-shell-base/linux-shell-base#installation'>Installation</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href='https://github.com/linux-shell-base/linux-shell-base#contributing'>Contributing</a>
</p>
<br>
<br>

**Linux-shell-base** is a resource to remove the incongruences of free and open source software, revive the [UNIX philosophy](https://en.wikipedia.org/wiki/Unix_philosophy#Eric_Raymond.E2.80.99s_17_Unix_Rules) and make computing easy (see the [background philosophy](https://github.com/linux-shell-base/linux-shell-base/wiki/Background-philosophy) to learn more). Its solutions target multiple application layer paradigms and adhere to one principle: remove an incongruence of free and open source software with respect to the fundamental principles of computing (i.e. the UNIX philosophy).

Its objective is achieved by allowing free and open source software to be more communicable and with solutions that adhere to the following rules:

* Use a standard approach
* Provide documentation
* Do not contain errors
* Do not contain deprecated or old-styled code
* Be independent of other solutions
* Include a source if exists
* Conform to a standard [guideline][wiki]

# Paradigms

The following is a list of the application layer paradigms targeted by *Linux-shell-base* with examples:

## 3rd party applications

Generic solutions for 3rd party applications

* [Generic utility functions for MySQL](bin/3rd_party_applications/database/mysqlutil)
* [Generic utility functions for MongoDB](bin/3rd_party_applications/database/mongodbutil)

## Android

Solutions for Android devices

* [Send an sms using an Android device.](bin/android/sms)
* [Watch and print X and Y screen tap coordinates of an Android device.](bin/android/getmobiletappos)

## Bash

Solutions for the Bourne Again Shell (Bash)

* [Bash array utilities](bin/bash/arrayutils.bash)
* [Bash date and time utilities](bin/bash/dateandtimeutils.bash)

## Main

Solutions related to core aspects of the Linux operating system *(e.g. file, networking, x11)* performing an action, divided into three sections:
  1. **With output**

  * [Archive a file or directory with almost any archive format.](bin/main/with_output/file/archive)

  2. **Without output**

  * [Move a window to the left or right monitor.](bin/main/without_output/x11/movewindtolftorrghtmntr)

  3. **Modules** - solutions used in conjuction with command-line programs

  * [Run a command in the background.](bin/main/modules/shell/runinbg)
  * [Run a command when files have changed in the current directory.](bin/main/modules/file/inotify)

## Main - output only

Solutions related to core aspects of the Linux operating system performing no actions and providing output, divided into three sections:
  1. **Single-value**

  * [Get the size of one or more files and/or directories as a plain number.](https://github.com/linux-shell-base/linux-shell-base/blob/master/one-liners/one-liners-output.bash)
  * [Get the ID of a window by PID (and other X11 window management solutions).](https://github.com/linux-shell-base/linux-shell-base/tree/master/bin/main-output_only/single-value#x11)

  2. **Multi-value**

  * [Print the paths of the subsubdirectories of the specified directory.](bin/main-output_only/multi-value/file/printsubsubdirpaths)

  3. **User**

  * [Display current host related information.](bin/main-output_only/user/networking/localhost)

## Mobile

Solutions for mobile devices

* [Mount and unmount an MTP device.](bin/mobile/mtp)

## Modules

Modules - solutions used in conjuction with command-line programs

* [Return a file for a command using one of two search methods: (1) Locate from a database; (2) Recursively find from the current or specified directory.](bin/modules/file/returnfileforcmd)
* [Execute a program with an action on the resulting window.](bin/modules/x11/exeprogwithwindact)

## Utilities

Utilities

* [Open a new terminal optionally with an initial command to run.](bin/utilities/general/newterm)
* [Execute a command in (or run the last command of) a terminal emulator.](bin/utilities/keybind/termcommand)

# Excluded solutions

The following is a list of types of solutions excluded from *Linux-shell-base*:

* File formatting or converting *(e.g. BMP to JPEG or CYMK colors to RGB colors)*
* Text manipulation
* OS or architecture specific

# Packaged utilities

*Linux-shell-base* has an [extension repository for *utilities* consisting of more than one file][packaged-utilities].

# Installation

As *Linux-shell-base* is not a framework, there is no installation process other than cloning the repository, however, essential solutions can be retrieved by downloading *install-essentials.sh* with the following command and running it.

It provides 16 of the current 60 scripts, 50 of the current 52 aliases and short-functions and 3 of the current 4 one-liners in *Linux-shell-base*. All solutions are downloaded to a single directory in the user's home directory.

```bash
wget https://raw.githubusercontent.com/linux-shell-base/linux-shell-base/install/install-essentials.sh \
&& chmod +x install-essentials.sh
```

# Contributing

*Linux-shell-base* is perhaps unlike any other repository. It does not correspond to the normal patterns of software development and it's objective is not to create new free and open source software but to revive the UNIX philosophy in it. As a result, a solution must be able to achieve exactly the same action or output regardless of implementation.

If you would like to help and contribute, please create a [pull request](https://gist.github.com/Chaser324/ce0505fbed06b947d962) and ensure that your solution adheres to the principle and general rules described above. If it does not conform to the respective [guideline][wiki], changes will be applied by *Linux-shell-base*. A contributed solution can be an alternative method/implementation to an already existing one. In this case, it will be given the same name with an incremented number.

Finally, credits will be placed in the wiki and can identify the user by name, username or URL.

Please send an email to *main@linuxshellbase.com* with any suggestions, comments or questions.



[packaged-utilities]: https://github.com/linux-shell-base/packaged-utilities
[wiki]: https://github.com/linux-shell-base/linux-shell-base/wiki
