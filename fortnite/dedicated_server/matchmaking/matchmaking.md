# - Create Session (I think)

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:session_id                 |
| METHOD          | POST                                                                                                                 |
| QUERY           |                                                                                                                      |
| BODY            |                                                                                                                      |

Exemple (Body):
```json
{
    "ownerId": "8D396E3DE68845AE8131D4840DC21170",
    "ownerName": "[DS]odyssey-EU-FR-TEST",
    "serverName": "[DS]odyssey-EU-FR-TEST",
    "maxPublicPlayers": 100,
    "maxPrivatePlayers": 0,
    "shouldAdvertise": false,
    "allowJoinInProgress": false,
    "isDedicated": true,
    "usesStats": false,
    "allowInvites": false,
    "usesPresence": false,
    "allowJoinViaPresence": true,
    "allowJoinViaPresenceFriendsOnly": false,
    "buildUniqueId": "4047718",
    "attributes": {
        "ALLOWMIGRATION_s": "false",
        "REJOINAFTERKICK_s": "OPEN",
        "CHECKSANCTIONS_s": "false",
        "STORMSHIELDDEFENSETYPE_i": 0,
        "BEACONPORT_i": 7777,
        "BUCKET_s": "EU:[DS]ODYSSEY-EU-FR-TEST:4047718:Fortnite",
        "DEPLOYMENT_s": "Fortnite",
        "LASTUPDATED_s": "2024-01-21T18: 34: 26.091Z",
        "PLAYLISTNAME_s": "playlist_defaultsolo",
        "LINKID_s": "playlist_defaultsolo",
        "DCID_s": "[DS]ODYSSEY-EU-FR-TEST",
        "ALLOWREADBYID_s": "false",
        "SERVERADDRESS_s": "127.0.0.1",
        "ALLOWBROADCASTING_b": true,
        "NETWORKMODULE_b": false,
        "HOTFIXVERSION_i": 1,
        "SUBREGION_s": "FR",
        "MATCHMAKINGPOOL_s": "Any",
        "SESSIONKEY_s": "B4D8A6D3C028400BB4434AD5C6BF432E",
        "REGION_s": "EU",
        "LINKTYPE_s": "BR:Playlist",
        "GAMEMODE_s": "FORTATHENA",
        "ADDRESS_s": "127.0.0.1"
    },
    "id": "711ac4cb63fe4725a2f5704d6c73634a",
    "serverAddress": "127.0.0.1",
    "serverPort": 7777,
    "openPrivatePlayers": 0,
    "openPublicPlayers": 100,
    "sortWeight": 0,
    "started": false,
    "publicPlayers": [],
    "privatePlayers": []
}
```

## RESPONSE
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| STATUS          | 204                                                                                                                  |

# - Delete Session

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:session_id                 |
| METHOD          | DELETE                                                                                                               |
| QUERY           |                                                                                                                      |
| BODY            |                                                                                                                      |

## RESPONSE
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| STATUS          | 204                                                                                                                  |

# - Add players in Session

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:session_id/players         |
| METHOD          | POST                                                                                                                 |
| QUERY           |                                                                                                                      |
| BODY            | publicPlayers, privatePlayers                                                                                        |

Exemple (Body):
```json
{
	"publicPlayers": [
        "7073004257a344e5b7bd8df2ed8e101a"
    ],
	"privatePlayers": []
}
```

## RESPONSE
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| STATUS          | 200                                                                                                                  |

Exemple (Response):
```json
{
    "maxPublicPlayers": 100,
    "openPublicPlayers": 99,
    "maxPrivatePlayers": 0,
    "openPrivatePlayers": 0,
    "publicPlayers": [
        "7073004257a344e5b7bd8df2ed8e101a"
    ],
    "privatePlayers": []
}
```

# - Remove players in Session

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:session_id/players         |
| METHOD          | DELETE                                                                                                               |
| QUERY           |                                                                                                                      |
| BODY            | Array                                                                                                                |

Exemple (Body):
```json
[
	"7073004257a344e5b7bd8df2ed8e101a"
]
```

## RESPONSE
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| STATUS          | 204                                                                                                                  |

# - Check players in Session (I think)

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:session_id/heartbeat       |
| METHOD          | POST                                                                                                                 |
| QUERY           |                                                                                                                      |
| BODY            |                                                                                                                      |

## RESPONSE
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| STATUS          | 204                                                                                                                  |