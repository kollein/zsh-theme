# Installation

### Fonts

  1. Download these four ttf files:
   - [MesloLGS NF Regular.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Regular.ttf)
   - [MesloLGS NF Bold.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold.ttf)
   - [MesloLGS NF Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Italic.ttf)
   - [MesloLGS NF Bold Italic.ttf](
       https://github.com/romkatv/powerlevel10k-media/raw/master/MesloLGS%20NF%20Bold%20Italic.ttf)
  2. Double-click on each file and click "Install". This will make `MesloLGS NF` font available to all
   applications on your system.
  3. Configure your terminal to use this font:
   - **Apple Terminal**: Open *Terminal → Preferences → Profiles → Text*, click *Change* under *Font*
     and select `MesloLGS NF` family.
   - **Visual Studio Code**: Open *File → Preferences → Settings* (PC) or
     *Code → Preferences → Settings* (Mac), enter `terminal.integrated.fontFamily` in the search box at
     the top of *Settings* tab and set the value below to `MesloLGS NF`.
     Consult [this screenshot](
       https://raw.githubusercontent.com/romkatv/powerlevel10k-media/389133fb8c9a2347929a23702ce3039aacc46c3d/visual-studio-code-font-settings.jpg)
     to see how it should look like or see [this issue](
       https://github.com/romkatv/powerlevel10k/issues/671) for extra information.

### Homebrew:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Theme: powerlevel10k
```
brew install romkatv/powerlevel10k/powerlevel10k
```

### Theme Configuration

- Create config file:
```
echo "source $(brew --prefix)/opt/powerlevel10k/powerlevel10k.zsh-theme" >>~/.zshrc
```
- Configure:
```
source ~/.zshrc
```

### ZSH Plugins
- Install zsh-autosuggestions:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```
- Install zsh-syntax-highlighting:
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```
Open the `~/.zshrc` file in editor and modify the plugins line like below:
```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```
Restart your terminal to see the result! :)