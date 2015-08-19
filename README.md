A Powerline style prompt for your shell
=======================================

A [Powerline](https://github.com/Lokaltog/vim-powerline) like prompt for Bash, without all the complicated bits.

### Bash:
Add the following to your `.bashrc`:

        function _update_ps1() {
           export PS1="$(~/powerline-shell.py $? 2> /dev/null)"
        }

        export PROMPT_COMMAND="_update_ps1; $PROMPT_COMMAND"