### o0th

<p align="center">
  <a>
    <img src="/assets/o0th.png" alt="screenshot">
  </a>
</p>

```bash
set -g @plugin 'o0th/tmux-nova'

set -g @nova-nerdfonts true
set -g @nova-nerdfonts-left 
set -g @nova-nerdfonts-right 

set -g @nova-segment-mode "#{?client_prefix,Ω,ω}"
set -g @nova-segment-mode-colors "#50fa7b #282a36"

set -g @nova-segment-whoami "#(whoami)@#h"
set -g @nova-segment-whoami-colors "#50fa7b #282a36"

set -g @nova-pane "#I#{?pane_in_mode,  #{pane_mode},}  #W"

set -g @nova-segment-spotify " #(spotifycli --status)"
set -g @nova-segment-spotify-colors "#282a36 #f8f8f2"

set -g @cpu_percentage_format "%5.1f%%"
set -g @nova-segment-cpu " #(~/.tmux/plugins/tmux-cpu/scripts/cpu_percentage.sh)"
set -g @nova-segment-cpu-colors "#282a36 #f8f8f2"

set -g @cpu_temp_unit "C"
set -g @cpu_temp_format "%3.0f"
set -g @nova-segment-cpu-temp "#(~/.tmux/plugins/tmux-cpu/scripts/cpu_temp.sh)"
set -g @nova-segment-cpu-temp-colors "#282a36 #f8f8f2"

set -g @ram_percentage_format "%5.1f%%"
set -g @nova-segment-ram "#(~/.tmux/plugins/tmux-cpu/scripts/ram_percentage.sh)"
set -g @nova-segment-ram-colors "#282a36 #f8f8f2"

set -g @gpu_percentage_format "%5.1f%%"
set -g @nova-segment-gpu "﬙ #(~/.tmux/plugins/tmux-cpu/scripts/gpu_percentage.sh)"
set -g @nova-segment-gpu-colors "#282a36 #f8f8f2"

set -g @gpu_temp_unit "C"
set -g @gpu_temp_format "%3.0f"
set -g @nova-segment-gpu-temp "#(~/.tmux/plugins/tmux-cpu/scripts/gpu_temp.sh)"
set -g @nova-segment-gpu-temp-colors "#282a36 #f8f8f2"

set -g @gram_percentage_format "%5.1f%%"
set -g @nova-segment-gram "#(~/.tmux/plugins/tmux-cpu/scripts/gram_percentage.sh)"
set -g @nova-segment-gram-colors "#282a36 #f8f8f2"

set -g @net_speed_interfaces "enp6s0"
set -g @net_speed_format "↓ %10s - ↑ %10s"
set -g @nova-segment-net "#(~/.tmux/plugins/tmux-net-speed/scripts/net_speed.sh)"
set -g @nova-segment-net-colors "#282a36 #f8f8f2"

set -g @nova-segment-pomodoro "#(pomodoro status --format ' %%c  %%r %%d') "
set -g @nova-segment-pomodoro-colors "#ff5555 #f8f8f2"

set -g @nova-rows 1
set -g @nova-segments-0-left "mode"
set -g @nova-segments-0-right "whoami pomodoro"
set -g @nova-segments-1-left "spotify"
set -g @nova-segments-1-right "cpu ram cpu-temp gpu gram gpu-temp"
```
