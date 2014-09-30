# Activities

Activity messages represent events in external services. That event could be a new user story for a project, an update to a support ticket or a commit to some repository, for example. Activities are always related to some entity which is represented by a [thread](Threads).

However, a comment or discussion in external services is represented by a separate [discussion](#/discussion) message.

<div id="/activity"></div>
## Activity

```
{
  "id": 13895827,
  "sent": 1411560930521,
  "event": "activity",
  "tags": [],
  "attachments": [],
  "flow": "ccc2899a-0485-4fd9-8706-e5bd28f03a9d",
  "author": {
    "name": "anttipitkanen",
    "avatar": "https://avatars.githubusercontent.com/u/946511?v=2"
  },
  "title": "Closed pull request",
  "body": null,
  "app": "influx",
  "user": 0,
  "edited": null,
  "content": null,
  "_application": 104,
  "_project": 220,
  "thread_id": "HbjDdeOqrZm6QzlSO8rwtftzwts",
  "thread": {
    "title": "Fix bug in thread API",
    "body": "",
    "external_url": "https://github.com/flowdock/component/pull/42",
    "status": {
      "color": "grey",
      "value": "closed"
    },
    "actions": [
      {
        "@type": "ViewAction",
        "url": "https://github.com/flowdock/component/pull/42/files",
        "name": "Diff",
        "description": "View diff in GitHub",
        "image": "https://s3.amazonaws.com/flowdock-resources/images/diff.png"
      }
    ],
    "fields": [],
    "source": {
      "id": 104,
      "icon": "https://fd-files-eu-qa.s3.amazonaws.com/applications/104/ef8eff491304914a.png",
      "application": "GitHub"
    },
    "activities": 3,
    "internal_comments": 3,
    "external_comments": 5
  }
}
```

<div id="/discussion"></div>
## Discussion

```
{
  "id": 13904478,
  "sent": 1411632833971,
  "event": "discussion",
  "tags": [],
  "attachments": [],
  "uuid": "nudVKk0wy79MTMk6URqJfw",
  "flow":"ccc2899a-0485-4fd9-8706-e5bd28f03a9d",
  "author": {
    "name": "Antti Pitk\u00e4nen",
    "avatar": "https://secure.gravatar.com/avatar/0d7d028dd0eec07add85a3bba314b456?s=120&r=pg",
    "email":"antti@flowdock.com"
  },
  "title": "replied",
  "body": "Message body with HTML formatting &lt;br&gt;&lt;br&gt;",
  "app": "influx",
  "user": "0",
  "edited": null,
  "content": null,
  "_application": 106,
  "_project":221,
  "thread_id": "zPEM5204zx5J9DwYI7BaU0eLk88",
  "thread": {
    "title": "Support request",
    "body": null,
    "external_url": "https://flowdock.zendesk.com/agent/#/tickets/6240",
    "status": {
      "value": "solved",
      "color": "grey"
    },
    "actions": [],
    "fields": [
      {
        "label": "Assignee",
        "value": "&lt;a href=\"mailto:antti@flowdock.com\" rel=\"nofollow\"&gt;Antti Pitk&auml;nen&lt;/a&gt;"
      },
      {
        "label": "Requester",
        "value": "&lt;a href=\"mailto:foo@example.com\" rel=\"nofollow\"&gt;John Smith&lt;/a&gt;"
      }
    ],
    "source": {
      "id": 106,
      "icon": "https://fd-files-eu-qa.s3.amazonaws.com/applications/106/6001f4814ff24487.png",
      "application": "Zendesk",
    },
    "activities": 0,
    "internal_comments": 2,
    "external_comments": 6
  }
}
```

##