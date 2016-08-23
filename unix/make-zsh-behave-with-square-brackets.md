Some tools (hello, Rake and Capistrano) use square brackets to pass parameters to tasks.

> cap production deploy[some-release-name]

If you're using `zsh`, it will try to expand the contents of the square brackets to a file. No bueno!

You can tell zsh to restrain itself with `noglob`

> noglob cap production deploy[some-release-name]
