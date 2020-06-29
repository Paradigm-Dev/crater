# Crater
Upcoming easy and powerful UI creation alternative to HTML that is based on JS. We wanted to create this lightweight package since we all hate HTML.

### Design we are hoping to use

#### HTML (required)
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Crater example</title>
    <script src="index.js" defer></script>
  </head>
  
  <body>
    <div id="app"></div>
  </body>
</html>
```
#### Javascript
```js
import crater from 'crater';

let C = crater.attach('#app');

C.class('some-sort-of-class')
  .border({
    color: C.colors.green,
    right: 3
  })
  .fontFamily('sans-serif');

C.div([
  C.p('Hello world!'),
  C.img('https://www.theparadigmdev.com/relay/img/paradigm.png)
    .padding({ bottom: 12 })
])
  .class('some-sort-of-class')
  .padding({ all: 0 })
  .margin({ top: 0 })
  .background({ color: C.colors.red })
  .color(C.colors.blue);
```
