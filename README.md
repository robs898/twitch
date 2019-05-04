### twitch_list
```
curl -s -H "Accept: application/vnd.twitchtv.v5+json" -H "Client-ID: <get from twitch api>" -X GET "https://api.twitch.tv/helix/streams/" | jq ".data[] | .user_name"
```

### twitch_play
```
function twitch_play {
        mpv "https://twitch.tv/$1"
}
```

### twitch_chat
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
