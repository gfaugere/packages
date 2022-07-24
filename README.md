# Packages

Repository to automate distribution of packages

## Distributed binaries

- `qad` ([quick-automation-devtool](https://gitlab.com/pag-station/quick-automation-devtool))

## Supported platforms

### Debian-based

```bash
curl https://gfaugere.gitlab.io/packages/debian/public_key.gpg | sudo apt-key add -
echo 'deb https://gfaugere.gitlab.io/packages/debian/ ./' | sudo tee -a /etc/apt/sources.list
sudo apt update
sudo apt install <package>
```

### rpm-based

```bash
sudo dnf config-manager --add-repo https://gfaugere.gitlab.io/packages/rpm/gfaugere-packages.repo
sudo dnf install <package>
```
