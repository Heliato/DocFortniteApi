# - Create Session (I think)

## REQUEST
| Title           | Body                                                                                                                 |         
| --------------- | -------------------------------------------------------------------------------------------------------------------- |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/matchmaking/session/:account_id/players         |
| METHOD          | POST                                                                                                                 |
| QUERY           |                                                                                                                      |
| BODY            | publicPlayers, privatePlayers                                                                                        |

Exemple (Body):
```json
{
	"publicPlayers": [],
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
    "openPublicPlayers": 100,
    "maxPrivatePlayers": 0,
    "openPrivatePlayers": 0,
    "publicPlayers": [],
    "privatePlayers": []
}
```