## Install `pyenv`

```
git clone https://github.com/pyenv/pyenv.git ~/.pyenv
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo 'export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo -e 'if command -v pyenv 1>/dev/null 2>&1; then\n  eval "$(pyenv init -)"\nfi' >> ~/.zshrc
```

## Install Python build dependancies

These are required to build and install most of packages

```
sudo apt install -y libssl1.1 libssl-dev libffi-dev
pyenv install 3.8.2
```

## Switch to Python and check the version

```
pyenv versions
pyenv global 3.8.2
```

## Hints

You don't need `sudo` to install packages globally, everything is in home folder now.
