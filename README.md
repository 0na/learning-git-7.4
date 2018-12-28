https://0na.github.io/learning-git-7.4/




Wszystkie polecenia zdaje się, że działają okej :
Air-Aleksandra:learning-git-7.4 aleksandra$ npm run watch

> learning-git-7.5@1.0.0 watch /Users/aleksandra/learning-git/learning-git-7.4
> npm-run-all build -p watch:*


> learning-git-7.5@1.0.0 build /Users/aleksandra/learning-git/learning-git-7.4
> npm run build:sass && npm run build:autoprefixer && npm run test


> learning-git-7.5@1.0.0 build:sass /Users/aleksandra/learning-git/learning-git-7.4
> node-sass --output-style compact -o css sass

Rendering Complete, saving .css file...
Wrote CSS to /Users/aleksandra/learning-git/learning-git-7.4/css/style.css
Wrote 1 CSS files to /Users/aleksandra/learning-git/learning-git-7.4/css

> learning-git-7.5@1.0.0 build:autoprefixer /Users/aleksandra/learning-git/learning-git-7.4
> autoprefixer-cli css/style.css


> learning-git-7.5@1.0.0 test /Users/aleksandra/learning-git/learning-git-7.4
> npm run test:html


> learning-git-7.5@1.0.0 test:html /Users/aleksandra/learning-git/learning-git-7.4
> globstar nu-html-checker *.html

index.html
10:10-131  error  Bad value “https://fonts.googleapis.com/css?family=Amatic+SC|Raleway:400,400i,700&subset=latin-ext” for attribute “href” on element “link”: Illegal character in query: “|” is not allowed.


> learning-git-7.5@1.0.0 watch:sassprefixer /Users/aleksandra/learning-git/learning-git-7.4
> onchange sass/*.scss -- npm-run-all -p build:sass build:autoprefixer


> learning-git-7.5@1.0.0 watch:sass /Users/aleksandra/learning-git/learning-git-7.4
> node-sass --output-style expanded --source-map true -o css sass --watch


> learning-git-7.5@1.0.0 watch:browsersync /Users/aleksandra/learning-git/learning-git-7.4
> browser-sync start --server --files css/*.css *.html

[Browsersync] Access URLs:
 ------------------------------------
       Local: http://localhost:3000
    External: http://192.168.1.5:3000
 ------------------------------------
          UI: http://localhost:3001
 UI External: http://localhost:3001
 ------------------------------------
[Browsersync] Serving files from: ./
[Browsersync] Watching files...
^C


