# MySuper development kit

...

## On OSX: install with Brew

Brew is a popular package manager on *macOS*.
However, it does not come pre-installed: follow the instructions from the Brew [Website](https://brew.sh/index_fr):

```sh
$ brew install git mise
```

Next, activate mise ([you can see official documentation](https://mise.jdx.dev/getting-started.html))

If you use **Bash** shell execute:

```sh
$ echo 'eval "$(~/.local/bin/mise activate bash)"' >> ~/.bashrc
$ source ~/.bash_profile
```

If you use **Zsh** shell execute:

```sh
$ echo 'eval "$(~/.local/bin/mise activate zsh)"' >> ~/.zshrc
$ source ~/.zsrhrc
```

```
$ mise install -y
```

## Configure direnv

If you use **Bash** shell execute:

```sh
$ echo -e "\neval \"\$(direnv hook bash)\"" >> ~/.bash_profile
$ source ~/.bash_profile
```

If you use **Zsh** shell execute:

```sh
$ echo -e "\neval \"\$(direnv hook zsh)\"" >> ~/.zshrc
$ source ~/.zsrhrc
```

More info see [direnv man page](https://direnv.net/#man/direnv.1)
