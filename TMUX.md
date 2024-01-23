# TMUX Terminal Commands

* Open Tmux session :
 ```
tmux
```

* Split terminal :
```
(shift + ctl) +(b+%)  (vertical)
(shift +ctl) + (b + ") (horizontal)
  
```

* Navigate in pans
   ```
  ctl + b + o (next)
  ctl + b + l (last)
  ctl + b + ->
  ctl +b + <-

    ```
* Close pan
  ```
  ctl + b + x
  ```
* Close tmux session

```
ctl + b + d
```
### Scrolling 

Ctrl-b then [ then you can use your normal navigation keys to scroll around (eg. Up Arrow or PgDn). Press q to quit scroll mode.

Alternatively you can press Ctrl-b PgUp to go directly into copy mode and scroll one page up (which is what it sounds like you will want most of the time)
You should consider the proper way to set scrolling: add in your ~/.tmux.conf


```
set -g mouse on        #For tmux version 2.1 and up
or

set -g mode-mouse on   #For tmux versions < 2.1
```
