---
title: contacts.search
description: Search contacts
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: contacts.search  
[Back to methods index](index.md)


Search contacts

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|q|[string](../types/string.md) | The search query | Yes|
|limit|[int](../types/int.md) | How many results should be returned | Yes|


### Return type: [contacts\_Found](../types/contacts_Found.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$contacts_Found = $MadelineProto->contacts->search(['q' => 'string', 'limit' => int, ]);
```

Or, if you're into Lua:

```lua
contacts_Found = contacts.search({q='string', limit=int, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|QUERY_TOO_SHORT|The query string is too short|
|400|SEARCH_QUERY_EMPTY|The search query is empty|
|-503|Timeout|Timeout while fetching data|

