# ng-kanban

## Create new project

Install the CLI using the npm package manager:

```
npm install -g @angular/cli
```

To create, build, and serve a new, basic Angular project on a development server, go to the parent directory of your new workspace use the following commands:

```
ng new my-first-project
cd my-first-project
ng serve
```

## Configure Mock Server

Add it to your dependencies using NPM:

```
npm i @mocks-server/main --save-dev
```

Add next script to your package.json file:

```
{
  "scripts": {
    "mocks" : "mocks-server"
  }
}
```

Now, you can start Mocks Server with the command:

```
npm run mocks
```

Get users:

```
curl http://localhost:3100/api/users
```

Get a specific user:

```
curl http://localhost:3100/api/users/1
```