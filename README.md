# Change the looks of your terminal following these simple installation guide

## 1. Install zsh
First you gotta need to download the zsh packages in any debain base
type the command ```sudo apt install zsh```

Then the zsh will be installed into your system...
After that enter zsh using the command ```zsh``` then choose option number 0,
then your system will create a dotfile called ~/.zshrc this file is where you can 
configure your zsh shell. 


You gotta install other auto highlighting and auto suggestions (This is totally optional)

## 2. Add the paths to your .zshrc file
```
source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
```
## 3. Install zsh auto complete from a github repository
You gotta download the auto complete of the zsh using the following git link

```https://github.com/marlonrichert/zsh-autocomplete```

The following command to clone it:

```% git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git```

Then add the source of that git repo into your own .zshrc config file

```source /path/to/zsh-autocomplete/zsh-autocomplete.plugin.zsh```

## 4. Install starship 
To download starship into your os ```curl -sS https://starship.rs/install.sh | sh```

And add ```eval "$(starship init zsh)"``` to the .zshrc file

to configure it make sure that in the ~ directory
you have a .config  ```mkdir -p ~/.config``` file and then use create a

 ```~/.config/starship.toml``` if it doesn't exist, then from the starships copy any liked I am using the following theme:

```starship preset catppuccin-powerline -o ~/.config/starship.toml```

And that's it for now <3..
