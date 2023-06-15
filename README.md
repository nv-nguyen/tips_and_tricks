# Tips and tricks
Some cools tips and tricks for coding that I learnt from my collaborators and labmates (for my personal uses).
- Bash hightlights with [Oh my bash](https://github.com/ohmybash/oh-my-bash)
```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/ohmybash/oh-my-bash/master/tools/install.sh)"
```
- Colors, tree views with [LSD](https://github.com/lsd-rs/lsd)
```
sudo snap install lsd
```
Then, adding alias to ~/.bashrc
```
# lsd
alias ls='lsd'
alias l='ls -l'
alias la='ls -a'
alias lla='ls -la'
alias lt='ls --tree'
```
- Conda and tmux alias
```
alias cn='conda create python=3.8.5 -n' # cn test
alias ca='conda activate' # ca test
alias cl='conda env list'

alias tn='tmux new -s' # tn a
alias ta='tmux attach -t' # ta a 
alias tl='tmux list-sessions'

alias cudaw='f(){ export CUDA_VISIBLE_DEVICES="$@" ;  unset -f f; }; f' # cudaw 0,1,2,3
alias cudar='echo $CUDA_VISIBLE_DEVICES'
alias ns='nvidia-smi'

# slurm alias
alias see_slurm='sattach -l' # see_slurm 1234.0 
```
- Tmux config
```
# Enable mouse control 
set -g mouse-select-window on
set -g mouse-select-pan

# switch panes using Alt-arrow without prefix 
bind -n M-Left select-pane -L
bind -n M-Right select-pane -R
bind -n M-Up select-pane -U
bind -n M-Down select-pane -D

# switch windows using shift-arrow without prefix 
bind -n S-Left previous-window
bind -n S-Right next-window
```

# Additional
- PhD's tips and tricks from [Yana Hasson](https://github.com/hassony2/useful-computer-vision-phd-resources) and [Thibault Groueix](https://github.com/ThibaultGROUEIX/useful-computer-vision-phd-resources) 
- SSH without password [gist](https://gist.github.com/slowkow/8798394)
- Hard disk partitions [makeuseof](https://www.makeuseof.com/tag/mounting-hard-disks-partitions-using-linux-command-line/)
- Meeting with advisors from [Jia-Bin Huang](https://threadreaderapp.com/thread/1418407079077842944.html)

- [How to write a good CVPR
  submission](https://billf.mit.edu/sites/default/files/documents/cvprPapers.pdf) by Bill Freeman.
- [How to write a bad article](https://people.csail.mit.edu/fredo/FredoBadWriting.pdf) by Fredo Durand
- [More ressources](https://people.csail.mit.edu/fredo/student.html) by Fredo Durand
