## Are you Tired of slow animation of dock in Mac?

#### ℹ️ Prerequisite
first make sure `Automatically hide and show the Dock` is toggled on in <br>settings -> desktop and dock 



[hii](https://github.com/user-attachments/assets/418f154b-4ea2-4e96-aa4c-f89fea86ab39)



#### 🤖 Command
To set the macOS Dock to hide and show instantly, execute the following command in your Terminal:
```
defaults write com.apple.dock autohide-time-modifier -int 0;
defaults write com.apple.dock autohide-delay -float 0;
killall Dock
```


https://github.com/user-attachments/assets/f6e9450d-da27-41fb-a22a-0409ac4e662e

#### 📄 Explanation:

`defaults write com.apple.dock autohide-time-modifier -int 0`

• This command sets the animation duration for showing or hiding the Dock to 0 seconds, making it appear or disappear instantly.

`defaults write com.apple.dock autohide-delay -float 0`

• This command removes the delay before the Dock starts hiding after your cursor moves away, making the hiding action immediate.

`killall Dock`

• This command restarts the Dock, applying the changes immediately.



#### ↩️ Reverting to Default behavior
If you decide to revert the Dock to its default settings, use the following command:
```
defaults delete com.apple.dock autohide-time-modifier; defaults delete com.apple.dock autohide-delay; killall Dock
```






