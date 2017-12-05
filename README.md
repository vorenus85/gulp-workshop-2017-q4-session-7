# Typescript compiler gulp task

Work to the <b>start</b> folder, the solutions are in the <b>end</b> folder

## 1. Npm init
type to terminal:

```$xslt
npm init
```

## 2. Modify package.json enrtypoint

```$xslt
"main": "dist/main.js"
```

## 3. Install packages

```$xslt
npm install --save-dev typescript gulp gulp-typescript
```

## 4. Deklare packages

```$xslt
var gulp = require("gulp");
var ts = require("gulp-typescript");
var tsProject = ts.createProject("tsconfig.json");
```
## 5. Create task

```$xslt
gulp.task("default", function () {
return tsProject.src()
.pipe(tsProject())
.js.pipe(gulp.dest("dist"));
```

## 6. Run default gulp task

```$xslt
gulp
```

## 7. Run main.js with node
Write to terminal
```$xslt
node dist/main.js
```

## 8. Open dist/main.js

## 9. Open tsconfig.json

change target parameter to ```ES3```

## 10. Run default gulp task

```$xslt
gulp
```
## 11. Run main.js with node
Write to terminal
```$xslt
node dist/main.js
```

## 12. Open again dist/main.js