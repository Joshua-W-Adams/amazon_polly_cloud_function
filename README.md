# TypeScript Project Boilerplate

A template for creating basic TypeScript projects

## Getting Started

1. Install Node.js

```
https://nodejs.org/en/download/
```

2. Clone repository to your system using the following command or git desktop

```shell
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY
```

3. Install repository dependencies

```shell
npm install
```

4. Run and lint Application

```shell
npm start
```

## Manual Setup Instructions

Alternatively a fresh project can be created by following the steps below.

1. Make new project directory

```shell
mkdir <project_name>
cd <project_name>
```

2. Initalise npm project

```shell
npm init
```

3. Install all TypeScript dependancies

```shell
npm install -D typescript
npm install -D tslint
npm install -D @types/node
```

Note: types/node required otherwise internal node libraries will not be detected by TypeScript.

4. Initialise TypeScript project

```shell
tsc init
```

5. Update typescript compilier with outpur directory for JavaScript files

```json
{
  "compilerOptions": {
    "outDir": "dist"
  },
}
```

6. Update package.json file with start up script to lint, compile and run app.

```json
"scripts": {
    "start": "tsc && node dist/app.js"
  }
```

7. Create application TypeScript file

```shell
touch src\app.ts
```

8. Compile and run TypeScript app

```shell
npm start
```
