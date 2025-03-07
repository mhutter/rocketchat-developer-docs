# Get Department by Unit Id

Gives departments included in a specific unit id

![](../../../../../../../.gitbook/assets/enterprise.jpg)

| URL                                         | Requires Auth | HTTP Method |
| ------------------------------------------- | ------------- | ----------- |
| `api/v1/livechat/units/:unitId/departments` | `YES`         | `GET`       |

## Headers

| Argument       | Example        | Required | Description                                                    |
| -------------- | -------------- | -------- | -------------------------------------------------------------- |
| `X-User-Id`    | `myuser-name`  | Required | Your username hash (returned after you log in through the API) |
| `X-Auth-Token` | `myauth-token` | Required | Your token (returned after you log in through the API)         |

## Path Variables

| Argument | Example             | Required | Description |
| -------- | ------------------- | -------- | ----------- |
| `unitId` | `sriw2wmP2Zz2pPrre` | Required | Unit Id     |

## Example Call

```bash
curl --location --request GET 'http://localhost:3000/api/v1/livechat/units/TGjc7wN84KxQup9cF/departments' \
--header 'X-Auth-Token: myauth-token' \
--header 'X-User-Id: myuser-name'
```

## Result

```javascript
{
    "departments": [
        {
            "_id": "MfvRXBwEWY6tTwqFh",
            "enabled": true,
            "name": "C",
            "description": "test dept",
            "showOnRegistration": true,
            "showOnOfflineForm": true,
            "requestTagBeforeClosingChat": true,
            "email": "C@test.com",
            "chatClosingTags": [
                "please add a tag"
            ],
            "offlineMessageChannelName": "",
            "maxNumberSimultaneousChat": "2",
            "visitorInactivityTimeoutInSeconds": "0",
            "abandonedRoomsCloseCustomMessage": "closed",
            "waitingQueueMessage": "please wait!",
            "departmentsAllowedToForward": "",
            "_updatedAt": "2022-12-14T14:44:51.923Z",
            "numAgents": 5,
            "ancestors": [
                "TGjc7wN84KxQup9cF"
            ],
            "parentId": "TGjc7wN84KxQup9cF",
            "fallbackForwardDepartment": "KgCzEB2gWngKp9JF3"
        }
    ],
    "count": 1,
    "offset": 0,
    "total": 1,
    "success": true
}
```
