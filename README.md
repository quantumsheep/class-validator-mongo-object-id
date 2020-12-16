# ObjectId Class Validator
This package validates ObjectId in classes. It was originally made to be used in NestJS but works everywhere else.

## How to install
```bash
npm install --save class-validator-mongo-object-id
```

## How to use
Here is an example along with commonly used `IsString` from [`class-validator`](https://github.com/typestack/class-validator) package.

```ts
import { IsString } from 'class-validator';
import { IsObjectId } from 'class-validator-mongo-object-id';

class EditUserDTO {
    @IsObjectId()
    userId: string;

    @IsString()
    username: string;
}
```
