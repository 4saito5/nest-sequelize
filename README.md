# nest-sequelize


## 環境構築ログ

```sh
# npm install -g npm@9.6.5
# npm i -g @nestjs/cli
nest new sample001

# ディレクトリ階層を1つ下げる
mv sample001/* .
mv sample001/.* . > /dev/null 2>&1
rm -rf sample001/

npm run start:dev
```

https://docs.nestjs.com/recipes/sql-sequelize
[Nest.jsでSequelizeを使ってみる](https://qiita.com/teracy164/items/2cea15e6abd560a4cea6)

```sh
npm install --save @nestjs/sequelize sequelize sequelize-typescript pg
npm install --save-dev @types/sequelize

mkdir database
touch database/database.config.ts
touch database/database.providers.ts
touch database/database.module.ts
touch database/cats.entity.ts
mkdir cats
touch cats/cats.providers.ts
touch cats/cats.module.ts
touch cats/cats.service.ts
touch cats/cats.controller.ts


npx sequelize-cli migration:generate --name init

```



[PostgreSQL と PGAdmin の docker-compose](https://qiita.com/Akhr/items/8d5b5127ee971a640253)  
pgadminでデータ作成  
http://localhost:8080  
example@example.com
test

http://localhost:8000/cats
