# Installing PyEnv
1. `brew install pyenv`
2. Add the following line to shell config file. `eval "$(pyenv init -)"`
3. `source <shell_profile>`
4. Run `echo $PATH` and verify that the PATH environment variable starts with `shims`. For example
```
/Users/jane.doe/.pyenv/shims:/Users/jane.doe/.local/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/opt/X11/bin:/usr/local/git/bin:/Users/jane.doe/bin
```

# Installing Python with PyEnv
1. `pyenv install 3.x.x`
2. List python versions install `pyenv versions`

# Installing Virtualenv
1. `brew install virtualenv`
2. `brew install pyenv-virtualenvwrapper`
3. Add following lines to shell config file and run `source ~/.zprofile`
```
export WORKON_HOME=$HOME/.virtualenvs
pyenv virtualenvwrapper_lazy
```
# Working on a python project
1. To use a particular python version `pyenv shell 3.9.4`
2. Create a new virtual environment project `mkvirtualenv <project_name>`
3. To exit virtual environment, run `deactivate`
4. To work in an exisiting environment run `workon <project_name>`
5. To generate a `requirements.txt` file, run `pip3 freeze > requirements.txt`. To install dependencies from a `requirements.txt` file, run `pip3 install -r /path/to/requirements.tx`
