# - Create Session (I think)

## REQUEST
|  URL            | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:account_id/players         |
|  METHOD         | POST                                                                                                                 |
|  QUERY          |                                                                                                                      |
|  BODY           | publicPlayers, privatePlayers                                                                                        |

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
|  STATUS         | 200                                                                                                                  |

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