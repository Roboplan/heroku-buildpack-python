# Heroku Buildpack: Python seed runner
Installs pip libs, run custom code, then removes them.

### Usage
The seed runner uses 3 scripts that should be placed inside the `seed_runner`
folder of your app.
- `install.txt` will be install with `pip -e` similar to `requirments.txt`
- `run.sh` will be run by bash between install and uninstall
- `uninstall.txt` will be uninstalled by `pip`
