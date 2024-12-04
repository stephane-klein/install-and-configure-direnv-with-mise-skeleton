# MySuper development kit

...

## Workspace installation and configuration

This development environment is based on [Mise](https://mise.jdx.dev/) and [direnv](https://direnv.net/).  
The starting point is *Mise*, which installs *direnv* and all other local dependencies (except *Docker*).

### On OSX: install Mise with Brew

Brew is a popular package manager on *macOS*.
However, it does not come pre-installed: follow the instructions from the Brew [Website](https://brew.sh/index_fr):

```sh
$ brew install git mise
```

### On Fedora: install Mise with dnf

Install with *dnf* ([see official Mise instructions](https://mise.jdx.dev/installing-mise.html#dnf))

```sh
$ dnf install -y dnf-plugins-core
$ dnf config-manager --add-repo https://mise.jdx.dev/rpm/mise.repo
$ dnf install -y mise
```

### Configure Mise

Next, activate *mise* ([you can see official documentation](https://mise.jdx.dev/getting-started.html))

If you use **Bash** shell execute:

```sh
$ echo 'eval "$(~/.local/bin/mise activate bash)"' >> ~/.bashrc
$ source ~/.bash_profile
```

If you use **Zsh** shell execute:

```sh
$ echo 'eval "$(~/.local/bin/mise activate zsh)"' >> ~/.zshrc
$ source ~/.zshrc
```

```
$ mise install -y
```

### Configure direnv

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

## Workspace usage

```sh
$ direnv allow
```

```
$ echo $HELLO_WORLD
foo
```
