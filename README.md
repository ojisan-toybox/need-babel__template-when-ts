# need-babel\_\_template-when-ts

TS&amp;React でハローワールドする時に babel\_\_template が必要かチェック

babel\_\_template にまつわるバグは起きなかった。が、どっちにしろ Set の定義は必要。

```
❯ yarn tsc main.ts --outFile bundle.js
yarn run v1.19.1
$ need-babel__template-when-ts/node_modules/.bin/tsc main.ts --outFile bundle.js
node_modules/@types/react/index.d.ts:388:23 - error TS2583: Cannot find name 'Set'. Do you need to change your target library? Try changing the `lib` compiler option to es2015 or later.

388         interactions: Set<SchedulerInteraction>,
                          ~~~


Found 1 error.

error Command failed with exit code 2.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
