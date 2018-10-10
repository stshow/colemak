# colemak
A brief README for transitioning to Colemak, an ergonomic alternative to QWERTY. Colemak is a built-in for most modern Linux distros, but custom XKB layouts are necessary to use Tarmak. 

## Standard US PC105 layout (QWERTY)

```
alias us='setxkbmap us && setxkbmap -option caps:backspace && xset r 66'
```

## Transition to Colemak: 

    1.) git clone https://github.com/DreymaR/BigBagKbdTrixXKB.git 
    2.) cd BigBagKbdTrixXKB 
    3.) bash install-dreymar-xmod.sh 
    
## Backup location:

    4.)  ls -lh /usr/share/X11/ # 'mv dbak-xkb* xkb' to restore. 
    
## Bash alias'

```
alias tarmak1="setxkbmap us -variant tarmak1__e  -option caps:backspace && xset r 66"
alias tarmak2="setxkbmap us -variant tarmak2__et  -option caps:backspace && xset r 66"
alias tarmak3="setxkbmap us -variant tarmak3__etr  -option caps:backspace && xset r 66"
alias tarmak4="setxkbmap us -variant tarmak4__etro  -option caps:backspace && xset r 66"
alias colemak='setxkbmap us -variant colemak -option caps:backspace && xset r 66'
```

##### Tested on Arch Linux (10/1/2018) and Ubuntu 18.04

## A more 'permanent' method

Use https://github.com/stshow/tarmak-cli (a fork of https://github.com/azmr/tarmak-cli 2018-10-10 ). 

Then run `localectl set-keymap tarmakN` (where `N` is numbers 1 - 4). 

##### Tested on Arch Linux (10/10/2018) with `/etc/vconsole.conf` default `KEYMAP=us`. 


The goal is to spend 1 - 3 weeks on each tarmak "level" and then finally to a full Colemak layout. 

##### Further reading

https://forum.colemak.com/topic/1858-learn-colemak-in-steps-with-the-tarmak-layouts/
