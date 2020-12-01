# Introduction

For now, this works for BelongsTo. Only "BelongsToWithCreate" is available, my plan in the future is to do "BlongsToMany" one. 


## Install

Add the repo to you composer.json:
```json
 "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/netsells/create-relation-on-resource"
        }
    ],
```

Run this command in your nova project:
`composer require netsells/create-relation-on-resource`

Usage:

```php
use Netsells\CreateRelationOnResource\BelongsToWithCreate;

public function fields(Request $request)
{
    return [
        BelongsToWithCreate::make('Language')->quickCreate(),
    ];
}
```

## Thanks to:
- [64robots/nova-fields](https://github.com/64robots/nova-fields/)
- [ali-awwad/create-relation-on-resource](https://github.com/ali-awwad/create-relation-on-resource)
