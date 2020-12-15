# my-zsh-setup

> I use Apple's Terminal, but this can also be done in other macOS terminal emulators like [iTerm2](https://hyper.is) or [Hyper](https://hyper.is).

<br>

**Example:**
<img src="https://github.com/sindresorhus/pure/blob/master/screenshot.png" width="800">

**Requirements:**
- [pure](https://github.com/sindresorhus/pure#oh-my-zsh)
- [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)
    - [Homebrew formula](https://formulae.brew.sh/formula/zsh-syntax-highlighting)
- [terminal-snazzy](https://github.com/sindresorhus/terminal-snazzy)

**Steps:**
1. Download pure, zsh-syntax-highlighting (brew), and terminal-snazzy
2. Open Terminal.app. Import the Snazzy.terminal file, then make Snazzy your default profile
3. Add these lines to the **end** of your .zshrc 
    ```
    # Add pure to $fpath, initialize the prompt system, choose pure
    fpath+=$HOME/.zsh/pure
    autoload -U promptinit; promptinit
    prompt pure

    # enable syntax highlighting for zsh
    source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
    ```
