# ``>_`` typewritten - a minimal, informative zsh prompt theme

Leaves all the room for what's important.
<img align="center" src="https://raw.githubusercontent.com/reobin/typewritten/master/media/demo.gif" alt="video" />

> Terminal is [iTerm2](https://iterm2.com/) — Font is [FiraCode](https://github.com/tonsky/FiraCode) — Terminal theme is [SpaceCamp](https://github.com/reobin/spacecamp-iterm)

## Features
- Current directory
- Current git branch
- Git status indicators:
  - ``?``     &nbsp; — untracked change(s);
  - ``+``     &nbsp; — staged change(s);
  - ``!``     &nbsp; — file(s) modified in the repo;
  - ``»``     &nbsp; — renamed file(s);
  - ``—``     &nbsp; — deleted file(s);
  - ``$``     &nbsp; — stashed change(s);
  - ``#``     &nbsp; — unmerged change(s);
  - ``•|``    — behind of remote branch;
  - ``|•``    — ahead of remote branch;
- Prompt color changes to red when an error return code is\
returned and code is displayed on the right
- Cursor customization
- Prompt layout customization
- Prompt cursor fix when exiting vim

## Installation
Clone the repository into your custom oh-my-zsh themes directory:
```shell
$ git clone https://github.com/reobin/typewritten.git $ZSH_CUSTOM/themes/typewritten
```

Symlink ``typewritten.zsh-theme`` to your oh-my-zsh custom themes directory:
```shell
ln -s "$ZSH_CUSTOM/themes/typewritten/typewritten.zsh-theme" "$ZSH_CUSTOM/themes/typewritten.zsh-theme"
```

Set ``ZSH_THEME="typewritten"`` in your ``.zshrc``.

## Cursor option
Default cursor is ``underscore``, but there is two more options: ``beam`` and ``block``.
They are both configured by adding the `TYPEWRITTEN_CURSOR` zsh variable to your ``.zshrc``:
```shell
export TYPEWRITTEN_CURSOR="beam"
```

## Prompt layout options
3 prompt layouts are available. To customize the prompt layout, add define the `TYPEWRITTEN_PROMPT_LAYOUT` variable in your `.zshrc` to one of following values : `singleline`, `multiline`, or `singleline_verbose`.

**singleline (default)**
```shell
> 
```

**multiline**
```shell
user@host
> 
```

**singleline verbose**
```shell
user@host >
```

## Contributors
* [@thbe](https://github.com/thbe)
* [@erikr](https://github.com/erikr)

## Screenshots
Multiline
<img src="https://raw.githubusercontent.com/reobin/typewritten/master/media/multiline.png" alt="multiline" />

Return code
<img src="https://raw.githubusercontent.com/reobin/typewritten/master/media/return_code.png" alt="return code" />
