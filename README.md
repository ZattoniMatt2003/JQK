# JQK
Create a laravel project

# For use the db use this json 
[
    {
        "id": "_pb_users_auth_",
        "name": "users",
        "type": "auth",
        "system": false,
        "schema": [
            {
                "system": false,
                "id": "users_name",
                "name": "name",
                "type": "text",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "min": null,
                    "max": null,
                    "pattern": ""
                }
            },
            {
                "system": false,
                "id": "users_avatar",
                "name": "avatar",
                "type": "file",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "mimeTypes": [
                        "image/jpeg",
                        "image/png",
                        "image/svg+xml",
                        "image/gif",
                        "image/webp"
                    ],
                    "thumbs": null,
                    "maxSelect": 1,
                    "maxSize": 5242880,
                    "protected": false
                }
            }
        ],
        "indexes": [],
        "listRule": "id = @request.auth.id",
        "viewRule": "id = @request.auth.id",
        "createRule": "",
        "updateRule": "id = @request.auth.id",
        "deleteRule": "id = @request.auth.id",
        "options": {
            "allowEmailAuth": true,
            "allowOAuth2Auth": true,
            "allowUsernameAuth": true,
            "exceptEmailDomains": null,
            "manageRule": null,
            "minPasswordLength": 8,
            "onlyEmailDomains": null,
            "onlyVerified": false,
            "requireEmail": false
        }
    },
    {
        "id": "rrdx27jng53acvq",
        "name": "music",
        "type": "base",
        "system": false,
        "schema": [
            {
                "system": false,
                "id": "p94qf63w",
                "name": "name",
                "type": "text",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "min": null,
                    "max": null,
                    "pattern": ""
                }
            },
            {
                "system": false,
                "id": "vzgojoqe",
                "name": "file",
                "type": "file",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "mimeTypes": [],
                    "thumbs": [],
                    "maxSelect": 1,
                    "maxSize": 5242880,
                    "protected": false
                }
            }
        ],
        "indexes": [],
        "listRule": null,
        "viewRule": null,
        "createRule": null,
        "updateRule": null,
        "deleteRule": null,
        "options": {}
    },
    {
        "id": "rae1c77zo4t6zka",
        "name": "playlists",
        "type": "base",
        "system": false,
        "schema": [
            {
                "system": false,
                "id": "a5ipawhp",
                "name": "playlistName",
                "type": "text",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "min": null,
                    "max": null,
                    "pattern": ""
                }
            },
            {
                "system": false,
                "id": "csucm7vd",
                "name": "user",
                "type": "relation",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "collectionId": "_pb_users_auth_",
                    "cascadeDelete": false,
                    "minSelect": null,
                    "maxSelect": 1,
                    "displayFields": null
                }
            },
            {
                "system": false,
                "id": "bhuyr4sh",
                "name": "music",
                "type": "relation",
                "required": false,
                "presentable": false,
                "unique": false,
                "options": {
                    "collectionId": "rrdx27jng53acvq",
                    "cascadeDelete": false,
                    "minSelect": null,
                    "maxSelect": null,
                    "displayFields": null
                }
            }
        ],
        "indexes": [],
        "listRule": null,
        "viewRule": null,
        "createRule": null,
        "updateRule": null,
        "deleteRule": null,
        "options": {}
    }
]
