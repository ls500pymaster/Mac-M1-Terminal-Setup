### Mac M1 Terminal Setup | Brew + iTerm2 + ZSH + Oh My Zsh

# Homebrew

![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/homebrew.jpeg?raw=true)

#### Download Homebrew from [here](https://brew.sh "here")
You need to have Homebrew installed. Homebrew requires Command Line Tools for Xcode. But if you don't have it, the installation will install it for you.

**Basic installation**

    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

Run to check brew.
```bash
brew help
```

# iTerm2

![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/iterm2.jpeg?raw=true)

**iTerm2** is a replacement for Terminal and the successor to iTerm. It works on Macs with macOS 10.14 or newer. iTerm2 brings the terminal into the modern age with features you never knew you always wanted.

#### Download iTerms2 from [here](https://iterm2.com/downloads.html "here")

**Basic installation using Brew**

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    
# ZSH

![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/zsh_term.png?raw=true)

**ZSH** is a shell designed for interactive use and it is also a powerful scripting language.
You can install it

    brew install zsh
Check 

    zsh --version

If your shell is not ZSH, run the following

    chsh -s /bin/zsh

Then restart your iTerm2 or open a new tab in iTerm2 and check it.

    echo $SHELL


# Oh My Zsh

![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/omz.png?raw=true)

#### Download Oh My Zsh from [here](https://github.com/ohmyzsh/ohmyzsh "here")

**Oh My Zsh** is an open-source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes.

**Basic installation**

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    
Update Oh My Zsh

    omz update

Oh-My-Zsh may overwrites ~/.zshrc, you need to add the path to brew. You need to add it before plugins. Use a text editor (Vim/VSCode/TextEdit):

    xport PATH=/opt/homebrew/bin:$PATH
    

# ???? Starship

![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/starship.png?raw=true)

#### Download Starship from [here](https://github.com/starship/starship "here")

**Starship**  is a cross-shell prompt build using rust language. This is a very minimal and blazingly fast terminal prompt. The key reason for its popularity is its customizability. You can easily customize it using a TOML config file.

**Basic installation**

    brew install starship
    
Add the following to your .zshrc

     eval "$(starship init zsh)"
	 
	 
Create config file for starship

    mkdir -p ~/.config && touch ~/.config/starship.toml

My starship.toml you can find [here](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/starship.toml "here").


![](https://github.com/ls500pymaster/Mac-M1-Terminal-Setup/blob/main/img/my_starship.png?raw=true)

    



