# trello-connector

https://stackoverflow.com/questions/47392985/trello-rest-api-to-get-all-trello-cards-which-user-is-able-to-view-edit-delete-u

```
$ curl "https://api.trello.com/1/members/me/boards&key=da8dfb6480df3[...]c8f569448224&token=ATTAa22fb557e8de1181eaeccb3a0a2[...]20c24c370e5d4139afb24552386&modelTypes=cards" | jq .

[
  {
    "id": "65d4912b201455540f253055",
    "nodeId": "ari:cloud:trello::board/workspace/65d48e71738d9c7951a3dd51/65d4912b201455540f253055",
    "name": "Test",
    "desc": "",
    "descData": null,
    "closed": false,
    "dateClosed": null,
    "idOrganization": "65d48e71738d9c7951a3dd51",
    "idEnterprise": null,
    "limits": {
      "attachments": {
        "perBoard": {
          "status": "ok",
          "disableAt": 36000,
          "warnAt": 28800
        },
        "perCard": {
          "status": "ok",
          "disableAt": 1000,
          "warnAt": 800
        }
      },
      "boards": {
        "totalMembersPerBoard": {
          "status": "ok",
          "disableAt": 1600,
          "warnAt": 1280
        },
        "totalAccessRequestsPerBoard": {
          "status": "ok",
          "disableAt": 4000,
          "warnAt": 3200
        }
      },
      "cards": {
        "openPerBoard": {
          "status": "ok",
          "disableAt": 5000,
          "warnAt": 4000
        },
        "openPerList": {
          "status": "ok",
          "disableAt": 5000,
          "warnAt": 4000
        },
        "totalPerBoard": {
          "status": "ok",
          "disableAt": 2000000,
          "warnAt": 1600000
        },
        "totalPerList": {
          "status": "ok",
          "disableAt": 1000000,
          "warnAt": 800000
        }
      },
      "checklists": {
        "perBoard": {
          "status": "ok",
          "disableAt": 1800000,
          "warnAt": 1440000
        },
        "perCard": {
          "status": "ok",
          "disableAt": 500,
          "warnAt": 400
        }
      },
      "checkItems": {
        "perChecklist": {
          "status": "ok",
          "disableAt": 200,
          "warnAt": 160
        }
      },
      "customFields": {
        "perBoard": {
          "status": "ok",
          "disableAt": 50,
          "warnAt": 40
        }
      },
      "customFieldOptions": {
        "perField": {
          "status": "ok",
          "disableAt": 50,
          "warnAt": 40
        }
      },
      "labels": {
        "perBoard": {
          "status": "ok",
          "disableAt": 1000,
          "warnAt": 800
        }
      },
      "lists": {
        "openPerBoard": {
          "status": "ok",
          "disableAt": 500,
          "warnAt": 400
        },
        "totalPerBoard": {
          "status": "ok",
          "disableAt": 3000,
          "warnAt": 2400
        }
      },
      "stickers": {
        "perCard": {
          "status": "ok",
          "disableAt": 70,
          "warnAt": 56
        }
      },
      "reactions": {
        "perAction": {
          "status": "ok",
          "disableAt": 900,
          "warnAt": 720
        },
        "uniquePerAction": {
          "status": "ok",
          "disableAt": 17,
          "warnAt": 14
        }
      }
    },
    "pinned": false,
    "starred": false,
    "url": "https://trello.com/b/FZVHtixg/test",
    "prefs": {
      "permissionLevel": "org",
      "hideVotes": false,
      "voting": "disabled",
      "comments": "members",
      "invitations": "members",
      "selfJoin": true,
      "cardCovers": true,
      "cardCounts": false,
      "isTemplate": false,
      "cardAging": "regular",
      "calendarFeedEnabled": false,
      "hiddenPluginBoardButtons": [],
      "switcherViews": [
        {
          "viewType": "Board",
          "enabled": true
        },
        {
          "viewType": "Table",
          "enabled": true
        },
        {
          "viewType": "Calendar",
          "enabled": false
        },
        {
          "viewType": "Dashboard",
          "enabled": false
        },
        {
          "viewType": "Timeline",
          "enabled": false
        },
        {
          "viewType": "Map",
          "enabled": false
        }
      ],
      "background": "65d47c34083edc94329a1c62",
      "backgroundColor": null,
      "backgroundImage": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/original/407cb4c454e12143b80a5990854276d7/photo-1708058885492-09ef26cd4af8",
      "backgroundTile": false,
      "backgroundBrightness": "dark",
      "backgroundImageScaled": [
        {
          "width": 140,
          "height": 93,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/140x93/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 256,
          "height": 171,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/256x171/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 480,
          "height": 320,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/480x320/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 960,
          "height": 640,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/960x640/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 1024,
          "height": 683,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/1024x683/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 1280,
          "height": 854,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/1280x854/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 1920,
          "height": 1280,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/1920x1280/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 2048,
          "height": 1366,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/2048x1366/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 2400,
          "height": 1600,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/2400x1600/130c4d91907af9a6d991722c5261f0b8/photo-1708058885492-09ef26cd4af8.jpg"
        },
        {
          "width": 2560,
          "height": 1707,
          "url": "https://trello-backgrounds.s3.amazonaws.com/SharedBackground/original/407cb4c454e12143b80a5990854276d7/photo-1708058885492-09ef26cd4af8"
        }
      ],
      "backgroundBottomColor": "#303a3c",
      "backgroundTopColor": "#a4a7aa",
      "canBePublic": true,
      "canBeEnterprise": true,
      "canBeOrg": true,
      "canBePrivate": true,
      "canInvite": true
    },
    "shortLink": "FZVHtixg",
    "subscribed": false,
    "labelNames": {
      "green": "",
      "yellow": "",
      "orange": "",
      "red": "",
      "purple": "",
      "blue": "",
      "sky": "",
      "lime": "",
      "pink": "",
      "black": "",
      "green_dark": "",
      "yellow_dark": "",
      "orange_dark": "",
      "red_dark": "",
      "purple_dark": "",
      "blue_dark": "",
      "sky_dark": "",
      "lime_dark": "",
      "pink_dark": "",
      "black_dark": "",
      "green_light": "",
      "yellow_light": "",
      "orange_light": "",
      "red_light": "",
      "purple_light": "",
      "blue_light": "",
      "sky_light": "",
      "lime_light": "",
      "pink_light": "",
      "black_light": ""
    },
    "powerUps": [],
    "dateLastActivity": "2024-02-20T11:50:32.081Z",
    "dateLastView": "2024-02-20T12:05:18.787Z",
    "shortUrl": "https://trello.com/b/FZVHtixg",
    "idTags": [],
    "datePluginDisable": null,
    "creationMethod": "automatic",
    "ixUpdate": "7",
    "templateGallery": null,
    "enterpriseOwned": false,
    "idBoardSource": null,
    "premiumFeatures": [
      "additionalBoardBackgrounds",
      "additionalStickers",
      "customBoardBackgrounds",
      "customEmoji",
      "customStickers",
      "plugins"
    ],
    "idMemberCreator": "5d7f645a5f4b702381603484",
    "memberships": [
      {
        "idMember": "5d7f645a5f4b702381603484",
        "memberType": "admin",
        "unconfirmed": false,
        "deactivated": false,
        "id": "65d4912b201455540f253060"
      }
    ]
  }
]
```
