---
title: "messages.getEmojiKeywordsLanguages"
description: "Get info about an emoji keyword localization"
grand_parent: "Telegram RPC API"
parent: "Methods"
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getEmojiKeywordsLanguages.html
---
# Method: messages.getEmojiKeywordsLanguages
[Back to methods index](index.html)



Get info about an emoji keyword localization

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|lang\_codes|Array of [string](/API_docs/types/string.html) | Language codes | Yes|


### Return type: [Vector\_of\_EmojiLanguage](/API_docs/types/EmojiLanguage.html)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

// PHP 8+ syntax, use an array on PHP 7.
$Vector_of_EmojiLanguage = $MadelineProto->messages->getEmojiKeywordsLanguages(lang_codes: ['string', 'string'], );
```

