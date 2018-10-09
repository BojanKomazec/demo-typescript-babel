# demo-typescript-babel
A demo app which demonstrates how Babel transpiles TypeScript.
Inspiration:
https://blogs.msdn.microsoft.com/typescript/2018/08/27/typescript-and-babel-7/

To run compilation:
```
npm run compile
```
...or run Babel manually (form the project's root directory):
```
npx babel ./src --out-dir output --extensions ".ts,.tsx"
```

To run the Node.js application:
```
npm run start
```
...or run Node manually:
```
node output/index.js
```
Examples:

```
C:\dev\github\demo-typescript-babel>npm run compile

> demo-typescript-babel@1.0.0 compile C:\dev\github\demo-typescript-babel
> babel ./src --out-dir output --extensions ".ts,.tsx"

Successfully compiled 1 file with Babel.
```
```
C:\dev\github\demo-typescript-babel>npm run start

> demo-typescript-babel@1.0.0 start C:\dev\github\demo-typescript-babel
> node output/index.js

Hello, world!
```

Locally installed packages:
```

C:\dev\github\demo-typescript-babel>npm list --depth=0
demo-typescript-babel@1.0.0 C:\dev\github\demo-typescript-babel
+-- @babel/cli@7.1.2
+-- @babel/core@7.1.2
+-- @babel/plugin-proposal-class-properties@7.1.0
+-- @babel/plugin-proposal-object-rest-spread@7.0.0
+-- @babel/preset-env@7.1.0
`-- @babel/preset-typescript@7.1.0
```

Note that package typescript is NOT installed (it's not required).