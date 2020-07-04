# sind


Simple interactive dialog for Bash 4+. Developed on Ubuntu 18+ through [UserLAnd on Android](https://play.google.com/store/apps/details?id=tech.ula).

[![Build Status](https://travis-ci.org/l3laze/sind.svg?branch=master)](https://travis-ci.org/l3laze/sind) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/3212c5503ee94a42adb04cd730304493)](https://www.codacy.com/manual/l3laze/sind?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=l3laze/sind&amp;utm_campaign=Badge_Grade) [![codecov](https://codecov.io/gh/l3laze/sind/branch/master/graph/badge.svg)](https://codecov.io/gh/l3laze/sind)

[![Generic badge](https://img.shields.io/badge/Made%20with-Bash-black.svg)](https://shields.io/) [![Only 32 Kb](https://badge-size.herokuapp.com/l3laze/sind/master/sind.sh)](https://github.com/l3laze/sind/blob/master/sind.sh)



## Usage

```sh
userChoice="$(./sind.sh -t Title -o 'Okay')"

printf "%s\n" "$userChoice"
```


##### Output:

```
Choose one...
-----------------------------------------------------------
(↑/j or ↓/k, Enter to choose)
Okay
Cancel < -- background of selected will be colored.
-----------------------------------------------------------
Cancel
```


----


## Installation


Download `sind.sh` and place in a directory that's available from your `$PATH` or to the project that you're working on. The best place is `~/bin` to make it available to the current user (though it may not exist by default). For a system-wide install `/usr/local/bin` is best, based on the [Linux filesystem hierarchy](https://linux.die.net/man/7/hier) and related answers on [StackExchange](https://unix.stackexchange.com/questions/8656/usr-bin-vs-usr-local-bin-on-linux).


----


## Credits


- [Alexander Klimetschek's Stack Exchange answer](https://unix.stackexchange.com/a/415155/310780)
- [mtfurlan's vi keybinding patch/idea](https://github.com/l3laze/sind/issues/1)


----


## Contributing


Please ensure your pull request adheres to the following guidelines:


- **Please [open an issue](https://github.com/l3laze/sind/issues) before creating any new features**, for discussion.
- Bug fixes & POSIX-friendly changes are more than welcome!
- Check your spelling and grammar (if applicable).
- Try to use a text editor that will remove trailing whitespace (though mine on mobile can't..lol).
- Pass [shellcheck.net](https://www.shellcheck.net/). It is tested on push by Travis-CI, but doing so while developing helps minimize senseless Travis builds which are a waste of their resources.


----


## License

This project is distributed under the MIT License.
