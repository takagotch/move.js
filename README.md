### move.js
---

```
component install visionmedia/move.js
npm install move-js

make move.min.js
make UGLIFY_FLAGS=--no-mangle
```

```
<script src='move.min.js'></script>
```

```
move('.square')
  .to(500, 200)
  .rotate(180)
  .scale(.5)
  .set('background-color', '#888')
  .set('border-color', 'black')
  .duration('2s')
  .skew(50, -10)
  .then()
    .set('opacity', 0)
    .duration('0.3s')
    .scale(0.1)
    .pop()
  .end();
  
'in': 'ease-in'
'out': 'ease-out'
'in-out': 'ease-in-out'
'snap': 'cubic-bezier(0,1,.5,1)'
'linear': 'cubic-bezier(0.250, 0.250, 0.750, 0.750)'
'ease-in-quad': 'cubic-bezier(0.250, 0.250, 0.750, 0.750)'
...
```

