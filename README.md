# myexit
A zenity exit dialog
===================
## Usage:
myexit -h : show help
myexit -v : print version and exit
myexit <your config file> : launch my exit with your config file instead of $HOME/.config/myexit.conf
myexit : execute myexit with config file located in $HOME/.config/myexit.conf
===================
## Configuration file:
Before start you must create a configuration file and put in default path ($HOME/.config/myexit.conf) or 
you must start the program with the configuration file (path and filename) parameter.

In configuration file you must specify this params:

title:'the title you want to appear in dialog'
text:'a text to show in dialog before selection'
actions:'action1' 'action2' 'Another Action'

where each action is what you shuld see in selection.
For each action you have to specify what to do if selected

action1:slock
Another Action:command for this action with params

if you want to add the cancel or an action that
do nothing simply do not add them, in the example
action2 do nothing.