# ic_cheat
## 1.create vm
```javascript
var vm = document.querySelector('.container').__vue__;
```
## 2.simple 100 times
```javascript
Array(100).fill().forEach(() => { const a = vm.elements[Math.floor(Math.random() * vm.elements.length)]; const b = vm.elements[Math.floor(Math.random() * vm.elements.length)]; console.log(`Crafting ${a.text} + ${b.text}`); vm.craft(a, b); });
```
