# Node_Test
Testes e TDD com Jester para aplicação no node, ensinados pela [RocketSeat](http://rocketseat.com.br/).

Instale as dependências utilizando:
```
yarn install
```

E ajuste no package.json o pretest, test e posttest conforme o OS que você estiver usando:
```
Windows:
    "pretest": "set NODE_ENV=test && sequelize db:migrate",
    "test": "set NODE_ENV=test && jest",
    "posttest": "set NODE_ENV=test && sequelize db:migrate:undo:all"
Mac:
    "pretest": "NODE_ENV=test sequelize db:migrate",
    "test": "NODE_ENV=test jest",
    "posttest": "NODE_ENV=test sequelize db:migrate:undo:all"
```
Interessante também você ter uma db de postgres, caso o sqlite não seja criado.
