# ic_cheat
## 1.create vm
```javascript
var vm = document.querySelector('.container').__vue__;
```
## 2.run
### simple 100 times
```javascript
Array(100).fill().forEach(() => { const a = vm.elements[Math.floor(Math.random() * vm.elements.length)]; const b = vm.elements[Math.floor(Math.random() * vm.elements.length)]; console.log(`Crafting ${a.text} + ${b.text}`); vm.craft(a, b); });
```
### fast fixed
```javascript
(async () => { for (let i = 0; i < 1e6; i++) { await new Promise(resolve => setTimeout(resolve, 0)); const a = vm.elements[Math.floor(Math.random() * vm.elements.length)]; const b = vm.elements[Math.floor(Math.random() * vm.elements.length)]; vm.craft(a, b); } })();
```
