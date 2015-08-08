# PHP version switcher for OSX

If you're on OSX with PHP installed via Brew, you may be looking for an easy way to switch between PHP versions (5.3, 5.4, 5.5, 5.6, etc). Well, this package is it.

Requirements:
 - Apache using mod_fastcgi
 - PHP-FPM with service loaded (Ex: cp /usr/local/opt/php70/homebrew.mxcl.php70.plist ~/Library/LaunchAgents/, ...)
 - Every PHP-FPM versions config set the the same socket

Installation:
```
git clone git@github.com:dag-io/sphp-osx.git
```

Add `/usr/local/bin` to your `$PATH`. If you use the Bash shell, you can do this by running this command:
```
echo 'export PATH="/usr/local/bin:$PATH"' >> $HOME/.bashrc
```
You may need to restart your shell for this to take effect.

Usage:
```
./sphp-osx/sphp 53
./sphp-osx/sphp 54
./sphp-osx/sphp 55
./sphp-osx/sphp 56
```

## Contributors

* @conradkleinespel
* @sebastienbarre
* @uzyn
