## [GoTTY](https://github.com/yudai/gott)
[GoTTY](https://github.com/yudai/gotty) is a simple command line tool that turns your CLI tools into web applications.

This a Debian based GoTTY docker image.
### Usage
```
docker run -it -p 8080:8080 eshizhan/gotty
```
default enabled options: **`--permit-write --random-url --reconnect /bin/bash`**
### Options
```
--address, -a                                                IP address to listen [$GOTTY_ADDRESS]
--port, -p "8080"                                            Port number to listen [$GOTTY_PORT]
--permit-write, -w                                           Permit clients to write to the TTY (BE CAREFUL) [$GOTTY_PERMIT_WRITE]
--credential, -c                                             Credential for Basic Authentication (ex: user:pass, default disabled) [$GOTTY_CREDENTIAL]
--random-url, -r                                             Add a random string to the URL [$GOTTY_RANDOM_URL]
--random-url-length "8"                                      Random URL length [$GOTTY_RANDOM_URL_LENGTH]
--tls, -t                                                    Enable TLS/SSL [$GOTTY_TLS]
--tls-crt "~/.gotty.crt"                                     TLS/SSL certificate file path [$GOTTY_TLS_CRT]
--tls-key "~/.gotty.key"                                     TLS/SSL key file path [$GOTTY_TLS_KEY]
--tls-ca-crt "~/.gotty.ca.crt"                               TLS/SSL CA certificate file for client certifications [$GOTTY_TLS_CA_CRT]
--index                                                      Custom index.html file [$GOTTY_INDEX]
--title-format "GoTTY - {{ .Command }} ({{ .Hostname }})"    Title format of browser window [$GOTTY_TITLE_FORMAT]
--reconnect                                                  Enable reconnection [$GOTTY_RECONNECT]
--reconnect-time "10"                                        Time to reconnect [$GOTTY_RECONNECT_TIME]
--once                                                       Accept only one client and exit on disconnection [$GOTTY_ONCE]
--permit-arguments                                           Permit clients to send command line arguments in URL (e.g. http://example.com:8080/?arg=AAA&arg=BBB) [$GOTTY_PERMIT_ARGUMENTS]
--close-signal "1"                                           Signal sent to the command process when gotty close it (default: SIGHUP) [$GOTTY_CLOSE_SIGNAL]
--config "~/.gotty"                                          Config file path [$GOTTY_CONFIG]
--version, -v                                                print the version
```
