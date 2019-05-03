# twitch-chat
minimal twitch chat

1. Go here and get an oauth token: https://twitchapps.com/tmi/
2. Install sic: `sudo xbps-install -S sic`
3. Start sic: `sic -h irc.chat.twitch.tv -n <twitch username> -k "<paste oauth token>"`
4. Join channel: `:j #clintstevens`

Example:
```shell
sic -h irc.chat.twitch.tv -n cool_user_1 -k "oauth:0rio43t8jgkrmsgsl4e3"
```
```
:j #clintstevens
```
