---
title: API
layout: rancher-api-v2-beta-default-v1.6
version: v1.6
lang: en
apiVersion: v2-beta
#redirect_from:
#  - /rancher/v1.6/zh/api/v2-beta/api-resources/snapshot/
---

## snapshot



### Resource Fields

#### Writeable Fields

Field | Type | Create | Update | Default | Notes
---|---|---|---|---|---
description | string | Optional | Yes | - | 
name | string | Optional | Yes | - | 


#### Read Only Fields

Field | Type   | Notes
---|---|---
accountId | [account]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/{{page.apiVersion}}/api-resources/account/)  | The unique identifier for the associated account
created | date  | The date of when the snapshot was created.
data | map[json]  | 
id | int  | The unique identifier for the snapshot
kind | string  | 
removeTime | date  | The date and time of when the snapshot was removed
removed | date  | The date of when the snapshot was removed
state | enum  | The current state of the snapshot. The options are `created`, `creating`, `removed`, `removing`, `requested`.
transitioning | enum  | Whether or not the snapshot is in a transitioning state
transitioningMessage | string  | The message to show while in a transitioning state
transitioningProgress | int  | The percentage remaining in the transitioning process of the snapshot
uuid | string  | The universally unique identifier for the snapshot. This will always be unique across Rancher installations.
volumeId | [volume]({{site.baseurl}}/rancher/{{page.version}}/{{page.lang}}/api/{{page.apiVersion}}/api-resources/volume/)  | 


<br>
