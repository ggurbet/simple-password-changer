# simple-password-changer - A small GUI utility to change passwords visually

Simple password changer enables users to change their passwords without using a terminal application or a more complicated graphical utility. This tool directly talks with PAM to change a user's password regardless of the mechanism below. Tool also runs required checks before and after changing the password and informs the user about the result.

## Requirements

Following packages / libraries are required in order to run the program.

- `python-2.7`: Since it's developed with it.
- `python-pexpect`: Used to talk with `passwd` command with complex conversations.
- `python-gi`: For the user interface.
- `python-gi-cairo`: For the user interface.
- `gir1.2-gtk-3.0`: For native rendering of UI.
- **Important:** Tool requires `en_US-utf8` locale to be *installed*. It doesn't have to be the default but it should be available when one runs `locale -a`.

## Installation steps

Tool is designed for easy installation. Just copy the files into their places.

### Before Starting

This tool relies on `PAM` configuration of the host system. Correct configuration of `PAM` is essential.

### File Locations

- `simple-password-changer`: `/usr/local/bin/simple-password-changer` (Since it can be used by regular users and it's not installed by a package).
- `simple-password-changer.desktop`: `/usr/share/applications/simple-password-changer.desktop` (To add the launcher to application menus).

Utility can be used after copying files. Menu update may require a logout/login.
