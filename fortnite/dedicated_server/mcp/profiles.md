# - Get Profile For Client

## REQUEST
| Title           | Body                                                                                                                           |         
| --------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| URL             | https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/game/v2/profile/:account_id/dedicated_server/QueryProfile |
| METHOD          | POST                                                                                                                           |
| QUERY           | profileId, rvn                                                                                                                 |
| BODY            |                                                                                                                                |

Exemple (Query):
```json
{
    "profileId": "common_public",
    "rvn": -1
}
```

Exemple (Body):
```json
{}
```

## RESPONSE
| Title           | Body                                                                                                                           |         
| --------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| STATUS          | 200                                                                                                                            |

Exemple (Response):
```json
{
    "profileRevision": 1,
    "profileId": "common_public",
    "profileChangesBaseRevision": 1,
    "profileChanges": [
        {
            "changeType": "fullProfileUpdate",
            "profile": {
                "created": "2024-01-03T17:49:22.186Z",
                "updated": "2024-01-03T17:49:22.186Z",
                "rvn": 1,
                "wipeNumber": 1,
                "accountId": "7073004257a344e5b7bd8df2ed8e101a",
                "profileId": "common_public",
                "version": "no_version",
                "stats": {
                    "attributes": {
                        "banner_color": "DefaultColor15",
                        "homebase_name": "",
                        "banner_icon": "SurvivalBannerStonewoodComplete"
                    }
                },
                "commandRevision": 0
            }
        }
    ],
    "profileCommandRevision": 0,
    "serverTime": "2024-01-21T18:43:53.682Z",
    "multiUpdate": [],
    "responseVersion": 1
}
```