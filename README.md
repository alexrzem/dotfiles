# dotfiles

https://github.com/bashdot/bashdot

## Install

MacOS Homebrew

```sh
brew tap bashdot/tap
brew install bashdot
```

## Quick Start

1. Create your initial profile directory, in this example, default.

    ```sh
    mkdir default
    ```

1. Add any files you would like symlinked into your home directory. For example:


    ```sh
    echo 'set -o vi' > default/env
    ```

    Note, bashdot **prepends a dot**, in front of the filename, to the linked file.


1. Install the profile.

    ```sh
    bashdot install default
    ```

    The above file **default/env** will now be linked to **~/.env**.

1. Continue adding your dotfiles.


   ```sh
   mv ~/.bashrc default/bashrc
   ```