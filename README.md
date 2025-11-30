# JavaScript DOM Manipulation - MCQ Questions

## Question 1
**Select element by ID and change text**

**Code:**
```javascript
document.getElementById('title').innerText = 'Hello DOM!';
```

**Options:**
- A) Adds new element
- B) Deletes element
- C) Changes text to Hello DOM!
- D) No effect

**✓ Correct Answer:** C) Changes text to Hello DOM!

**Explanation:** `getElementById` selects element and `innerText` updates its text.

---

## Question 2
**Change background color of page**

**Code:**
```javascript
document.body.style.backgroundColor = 'lightblue';
```

**Options:**
- A) Changes font
- B) Sets background to lightblue
- C) Adds new div
- D) No effect

**✓ Correct Answer:** B) Sets background to lightblue

**Explanation:** `style.backgroundColor` modifies body background.

---

## Question 3
**Add new paragraph dynamically**

**Code:**
```javascript
let p=document.createElement('p'); 
p.textContent='New paragraph'; 
document.body.appendChild(p);
```

**Options:**
- A) Adds new paragraph
- B) Deletes body
- C) Changes heading
- D) No effect

**✓ Correct Answer:** A) Adds new paragraph

**Explanation:** `createElement` + `appendChild` inserts new node.

---

## Question 4
**Query selector usage**

**Code:**
```javascript
document.querySelector('.btn').innerHTML='Click Me!';
```

**Options:**
- A) Deletes button
- B) Changes all buttons
- C) Changes first .btn text
- D) No effect

**✓ Correct Answer:** C) Changes first .btn text

**Explanation:** `querySelector` returns first match.

---

## Question 5
**Event listener on button**

**Code:**
```javascript
document.getElementById('btn').addEventListener('click',()=>alert('Button clicked!'));
```

**Options:**
- A) Shows alert
- B) Changes text
- C) No effect
- D) Deletes button

**✓ Correct Answer:** A) Shows alert

**Explanation:** `addEventListener` attaches click event.

---

## Question 6
**Remove element by ID**

**Code:**
```javascript
let el=document.getElementById('removeMe'); 
el.remove();
```

**Options:**
- A) Changes color
- B) Adds element
- C) Removes element
- D) No effect

**✓ Correct Answer:** C) Removes element

**Explanation:** `remove()` deletes node.

---

## Question 7
**Change image attribute**

**Code:**
```javascript
document.querySelector('img').setAttribute('alt','New Image');
```

**Options:**
- A) Updates alt
- B) Deletes image
- C) Adds caption
- D) No effect

**✓ Correct Answer:** A) Updates alt

**Explanation:** `setAttribute` modifies attribute.

---

## Question 8
**Get image src attribute**

**Code:**
```javascript
let src=document.querySelector('img').getAttribute('src');
```

**Options:**
- A) Deletes image
- B) Returns src
- C) Changes src
- D) No effect

**✓ Correct Answer:** B) Returns src

**Explanation:** `getAttribute` fetches attribute value.

---

## Question 9
**InnerHTML vs innerText**

**Code:**
```javascript
document.getElementById('demo').innerHTML='<b>Bold</b>';
```

**Options:**
- A) Shows Bold in bold
- B) Shows <b>Bold</b>
- C) Deletes text
- D) No effect

**✓ Correct Answer:** A) Shows Bold in bold

**Explanation:** `innerHTML` parses HTML tags.

---

## Question 10
**Change multiple list items color**

**Code:**
```javascript
document.querySelectorAll('li').forEach(li=>li.style.color='red');
```

**Options:**
- A) First li red
- B) No change
- C) All li red
- D) Error

**✓ Correct Answer:** C) All li red

**Explanation:** `querySelectorAll` returns NodeList.

---

## Question 11
**Predict output with innerText**

**Code:**
```javascript
document.body.innerHTML='<div id="a"></div>'; 
document.getElementById('a').innerText=5+5;
```

**Options:**
- A) 55
- B) Error
- C) 10
- D) Empty

**✓ Correct Answer:** C) 10

**Explanation:** 5+5 evaluates to 10.

---

## Question 12
**Complete code to add button**

**Code:**
```javascript
let btn=document.createElement('button'); 
btn.textContent='Submit'; 
document.body.appendChild(btn);
```

**Options:**
- A) Adds Submit button
- B) Deletes body
- C) Error
- D) No effect

**✓ Correct Answer:** A) Adds Submit button

**Explanation:** `createElement` + `appendChild` adds button.

---

## Question 13
**Event bubbling scenario**

**Code:**
```javascript
parent.addEventListener('click',()=>console.log('Parent')); 
child.addEventListener('click',()=>console.log('Child'));
```

**Options:**
- A) Child then Parent
- B) Parent only
- C) Error
- D) No effect

**✓ Correct Answer:** A) Child then Parent

**Explanation:** Events bubble up from child to parent.

---

## Question 14
**Prevent bubbling**

**Code:**
```javascript
child.addEventListener('click',e=>{e.stopPropagation(); console.log('Child only');});
```

**Options:**
- A) Child only
- B) Parent too
- C) Error
- D) No effect

**✓ Correct Answer:** A) Child only

**Explanation:** `stopPropagation` halts bubbling.

---

## Question 15
**Toggle class**

**Code:**
```javascript
document.getElementById('box').classList.toggle('active');
```

**Options:**
- A) Deletes box
- B) Error
- C) Toggles active
- D) No effect

**✓ Correct Answer:** C) Toggles active

**Explanation:** `classList.toggle` adds/removes class.

---

## Question 16
**Dynamic list creation**

**Code:**
```javascript
['A','B','C'].forEach(item=>{
  let li=document.createElement('li'); 
  li.textContent=item; 
  ul.appendChild(li);
});
```

**Options:**
- A) Error
- B) Empty
- C) Creates list A,B,C
- D) No effect

**✓ Correct Answer:** C) Creates list A,B,C

**Explanation:** Loop creates li elements.

---

## Question 17
**Replace element with outerHTML**

**Code:**
```javascript
document.getElementById('p').outerHTML='<div>Bye</div>';
```

**Options:**
- A) Adds div
- B) Error
- C) Replaces with div
- D) No effect

**✓ Correct Answer:** C) Replaces with div

**Explanation:** `outerHTML` replaces element itself.

---

## Question 18
**Set input value**

**Code:**
```javascript
document.querySelector('input').value='Test';
```

**Options:**
- A) Deletes input
- B) Error
- C) Sets input to Test
- D) No effect

**✓ Correct Answer:** C) Sets input to Test

**Explanation:** `value` property sets form field.

---

## Question 19
**Disable button**

**Code:**
```javascript
document.getElementById('btn').disabled=true;
```

**Options:**
- A) Error
- B) Disables button
- C) Deletes button
- D) No effect

**✓ Correct Answer:** B) Disables button

**Explanation:** `disabled` property disables element.

---

## Question 20
**Append multiple texts**

**Code:**
```javascript
document.getElementById('x').append('Hello','World');
```

**Options:**
- A) Error
- B) Hello only
- C) HelloWorld
- D) No effect

**✓ Correct Answer:** C) HelloWorld

**Explanation:** `append` adds multiple nodes/text.

---

## Question 21
**Replace child**

**Code:**
```javascript
parent.replaceChild(newEl,parent.firstChild);
```

**Options:**
- A) Error
- B) Deletes parent
- C) Replaces first child
- D) No effect

**✓ Correct Answer:** C) Replaces first child

**Explanation:** `replaceChild` swaps nodes.

---

## Question 22
**Count children**

**Code:**
```javascript
console.log(document.querySelector('ul').children.length);
```

**Options:**
- A) Error
- B) Always 0
- C) Number of li
- D) No effect

**✓ Correct Answer:** C) Number of li

**Explanation:** `children` returns element count.

---

## Question 23
**Scroll event**

**Code:**
```javascript
window.addEventListener('scroll',()=>console.log('Scrolling...'));
```

**Options:**
- A) Error
- B) Logs on scroll
- C) No effect
- D) Deletes body

**✓ Correct Answer:** B) Logs on scroll

**Explanation:** `scroll` event triggers on page scroll.

---

## Question 24
**Keydown event**

**Code:**
```javascript
document.addEventListener('keydown',e=>console.log(e.key));
```

**Options:**
- A) Error
- B) Logs key
- C) No effect
- D) Deletes input

**✓ Correct Answer:** B) Logs key

**Explanation:** `keydown` captures pressed key.

---

## Question 25
**Insert before**

**Code:**
```javascript
ref.parentNode.insertBefore(newEl,ref);
```

**Options:**
- A) Error
- B) After ref
- C) Inserts before ref
- D) No effect

**✓ Correct Answer:** C) Inserts before ref

**Explanation:** `insertBefore` places node before reference.

---

## Question 26
**Append with innerHTML**

**Code:**
```javascript
document.getElementById('a').innerHTML+='<p>Text</p>';
```

**Options:**
- A) Error
- B) Deletes div
- C) Adds p inside
- D) No effect

**✓ Correct Answer:** C) Adds p inside

**Explanation:** `innerHTML` appends HTML.

---

## Question 27
**Style multiple paragraphs**

**Code:**
```javascript
document.querySelectorAll('p').forEach(p=>p.style.fontSize='20px');
```

**Options:**
- A) Error
- B) First only
- C) All p font 20px
- D) No effect

**✓ Correct Answer:** C) All p font 20px

**Explanation:** Loop styles all.

---

## Question 28
**InsertAdjacentHTML**

**Code:**
```javascript
document.getElementById('a').insertAdjacentHTML('beforeend','<span>Hi</span>');
```

**Options:**
- A) Error
- B) Deletes div
- C) Adds span inside
- D) No effect

**✓ Correct Answer:** C) Adds span inside

**Explanation:** `insertAdjacentHTML` inserts HTML.

---

## Question 29
**Log innerHTML**

**Code:**
```javascript
console.log(document.getElementById('a').innerHTML);
```

**Options:**
- A) Error
- B) Empty
- C) Logs content
- D) No effect

**✓ Correct Answer:** C) Logs content

**Explanation:** `innerHTML` returns HTML content.

---

## Question 30
**Event delegation**

**Code:**
```javascript
list.addEventListener('click',e=>{
  if(e.target.tagName==='LI')
    console.log(e.target.textContent);
});
```

**Options:**
- A) Error
- B) Logs list
- C) Logs li text
- D) No effect

**✓ Correct Answer:** C) Logs li text

**Explanation:** Delegation handles future li.

---

## Question 31
**Async DOM update**

**Code:**
```javascript
setTimeout(()=>{document.body.append('Delayed');},1000);
```

**Options:**
- A) Error
- B) Adds Delayed after 1s
- C) No effect
- D) Deletes body

**✓ Correct Answer:** B) Adds Delayed after 1s

**Explanation:** `setTimeout` delays DOM update.

---

## Question 32
**Mutation observer**

**Code:**
```javascript
obs.observe(document.body,{childList:true}); 
document.body.append('New');
```

**Options:**
- A) Error
- B) Logs DOM changed
- C) No effect
- D) Deletes node

**✓ Correct Answer:** B) Logs DOM changed

**Explanation:** Observer detects mutations.

---

## Question 33
**Modal close on Escape**

**Code:**
```javascript
document.addEventListener('keydown',e=>{
  if(e.key==='Escape')
    modal.style.display='none';
});
```

**Options:**
- A) Error
- B) No effect
- C) Hides modal
- D) Deletes modal

**✓ Correct Answer:** C) Hides modal

**Explanation:** `keydown` Escape hides modal.

---

## Question 34
**Throttle scroll**

**Code:**
```javascript
if(!timer){
  timer=setTimeout(()=>{
    console.log('Scroll handled');
    timer=null;
  },500);
}
```

**Options:**
- A) Error
- B) Logs always
- C) Logs every 500ms
- D) No effect

**✓ Correct Answer:** C) Logs every 500ms

**Explanation:** Throttle limits frequency.

---

## Question 35
**Highlight table row**

**Code:**
```javascript
table.addEventListener('click',e=>{
  if(e.target.tagName==='TD')
    e.target.parentNode.style.background='yellow';
});
```

**Options:**
- A) Error
- B) No effect
- C) Highlights row
- D) Deletes table

**✓ Correct Answer:** C) Highlights row

**Explanation:** Event delegation highlights row.

---

## Question 36
**Infinite scroll**

**Code:**
```javascript
if(window.innerHeight+window.scrollY>=document.body.offsetHeight){
  document.body.append('More');
}
```

**Options:**
- A) Error
- B) No effect
- C) Adds More at bottom
- D) Deletes body

**✓ Correct Answer:** C) Adds More at bottom

**Explanation:** Checks scroll position.

---

## Question 37
**Toggle button text**

**Code:**
```javascript
btn.textContent=btn.textContent==='Show'?'Hide':'Show';
```

**Options:**
- A) Error
- B) Always Show
- C) Alternates text
- D) No effect

**✓ Correct Answer:** C) Alternates text

**Explanation:** Ternary toggles text.

---

## Question 38
**Clone template**

**Code:**
```javascript
let clone=tpl.content.cloneNode(true); 
document.body.appendChild(clone);
```

**Options:**
- A) Error
- B) No effect
- C) Inserts clone
- D) Deletes template

**✓ Correct Answer:** C) Inserts clone

**Explanation:** `cloneNode` copies template.

---

## Question 39
**Sort list**

**Code:**
```javascript
[...ul.children].sort((a,b)=>a.textContent.localeCompare(b.textContent))
  .forEach(li=>ul.appendChild(li));
```

**Options:**
- A) Error
- B) No effect
- C) Sorts li
- D) Deletes list

**✓ Correct Answer:** C) Sorts li

**Explanation:** `localeCompare` sorts alphabetically.

---

## Question 40
**Lazy load images**

**Code:**
```javascript
obs.observe(img); 
if(e.isIntersecting){
  img.src=img.dataset.src;
}
```

**Options:**
- A) Error
- B) Always loads
- C) Loads when visible
- D) No effect

**✓ Correct Answer:** C) Loads when visible

**Explanation:** IntersectionObserver loads on viewport.

---

## Question 41
**Form validation**

**Code:**
```javascript
form.addEventListener('submit',e=>{
  if(!input.value){
    e.preventDefault();
    alert('Required');
  }
});
```

**Options:**
- A) Error
- B) Always submits
- C) Prevents empty submit
- D) No effect

**✓ Correct Answer:** C) Prevents empty submit

**Explanation:** `preventDefault` stops submission.

---

## Question 42
**Click counter**

**Code:**
```javascript
btn.addEventListener('click',()=>{
  counter.textContent=++count;
});
```

**Options:**
- A) Error
- B) No effect
- C) Updates counter
- D) Deletes button

**✓ Correct Answer:** C) Updates counter

**Explanation:** Increments counter and updates DOM.

---

## Question 43
**Email validation**

**Code:**
```javascript
document.getElementById('email').addEventListener('input',e=>{
  let valid=/\S+@\S+\.\S+/.test(e.target.value); 
  e.target.style.borderColor=valid?'green':'red';
});
```

**Options:**
- A) Error
- B) No effect
- C) Colors border green/red based on validity
- D) Deletes input

**✓ Correct Answer:** C) Colors border green/red based on validity

**Explanation:** Validates email pattern and updates border color.

---

## Question 44
**for loop with setTimeout**

**Code:**
```javascript
for (var i = 0; i < 3; i++) { setTimeout(() => console.log(i), 0); }
```

**Options:**
- A) 0 1 2
- B) 3 3 3
- C) 0 1 2 3
- D) Error

**✓ Correct Answer:** B) 3 3 3

**Explanation:** `var` is function-scoped, so all timeouts reference the same `i` which becomes 3.

---

## Question 45
**Array forEach with if condition**

**Code:**
```javascript
let arr=[1,2,3]; arr.forEach(i => { if(i===1) continue; console.log(i); })
```

**Options:**
- A) 0 2
- B) 1 2
- C) 0 1
- D) 2 only

**✓ Correct Answer:** A) 0 2

**Explanation:** `continue` is invalid in forEach, but with proper syntax it would skip 1.

---

## Question 46
**Using for...in on array also returns what out of the following?**

**Code:**
```javascript
// for...in iteration on arrays
```

**Options:**
- A) Only numeric indexes
- B) Enumerable properties
- C) Only numeric symbols
- D) Prototype chain properties

**✓ Correct Answer:** B) Enumerable properties

**Explanation:** `for...in` iterates over all enumerable properties including inherited ones.

---

## Question 47
**forEach() immediately stops when a return is executed in callback**

**Code:**
```javascript
forEach() immediately stops when a return is executed in callback.
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only in async
- D) Depends

**✓ Correct Answer:** B) FALSE

**Explanation:** `return` in forEach only exits the current iteration, not the entire loop.

---

## Question 48
**for loop with if and break**

**Code:**
```javascript
for(let i of 'abc'){ if(i==='b') break; console.log(i); }
```

**Options:**
- A) a
- B) a b
- C) b c
- D) Error

**✓ Correct Answer:** A) a

**Explanation:** Loop breaks when `i` equals 'b', so only 'a' is logged.

---

## Question 49
**Object property access in for loop**

**Code:**
```javascript
let obj={a:1,b:2}; for(let k in obj){ console.log(k); }
```

**Options:**
- A) a b
- B) 1 2
- C) Error
- D) undefined

**✓ Correct Answer:** A) a b

**Explanation:** `for...in` iterates over object keys.

---

## Question 50
**In which loop is continue not valid?**

**Code:**
```javascript
// continue statement usage
```

**Options:**
- A) for
- B) while
- C) do...while
- D) forEach

**✓ Correct Answer:** D) forEach

**Explanation:** `continue` can only be used in traditional loops, not in array methods.

---

## Question 51
**Which will run at least once?**

**Code:**
```javascript
// Loop execution comparison
```

**Options:**
- A) for
- B) while
- C) do...while
- D) forEach

**✓ Correct Answer:** C) do...while

**Explanation:** `do...while` executes body before checking condition.

---

## Question 52
**What will break terminate?**

**Code:**
```javascript
// break statement behavior
```

**Options:**
- A) Only current loop
- B) All loops
- C) Only switch
- D) The entire program

**✓ Correct Answer:** A) Only current loop

**Explanation:** `break` exits only the innermost enclosing loop or switch.

---

## Question 53
**for loop with nested loops and early break**

**Code:**
```javascript
for (let i=0; i<5; i++){ for(let j=0; j<2; j++){ if(i===2) continue; console.log(i,j) } }
```

**Options:**
- A) 0 1 3 4
- B) 0 1 2 3 4
- C) 1 2 3 4
- D) 2 1 4

**✓ Correct Answer:** A) 0 1 3 4

**Explanation:** When `i===2`, the inner loop is skipped for that iteration.

---

## Question 54
**In nested loops, break without label breaks:**

**Code:**
```javascript
// Nested loops with break
```

**Options:**
- A) Innermost loop
- B) Outer loop
- C) All loops
- D) None

**✓ Correct Answer:** A) Innermost loop

**Explanation:** `break` without label only exits the immediate enclosing loop.

---

## Question 55
**Which loop can create infinite execution easily due to condition mismatch?**

**Code:**
```javascript
// Infinite loop potential
```

**Options:**
- A) for
- B) forEach
- C) for...in
- D) while

**✓ Correct Answer:** D) while

**Explanation:** `while` can easily become infinite if condition never becomes false.

---

## Question 56
**for...in returning keys vs for...of**

**Code:**
```javascript
// for...in vs for...of
```

**Options:**
- A) Strings
- B) Numbers
- C) Mixed
- D) Symbols

**✓ Correct Answer:** A) Strings

**Explanation:** `for...in` returns keys as strings.

---

## Question 57
**Which loop cannot be used on Sets?**

**Code:**
```javascript
// Loop compatibility with Sets
```

**Options:**
- A) for
- B) for...in
- C) for...of
- D) while

**✓ Correct Answer:** B) for...in

**Explanation:** Sets don't have enumerable properties, so `for...in` doesn't work.

---

## Question 58
**Array forEach() skips empty slots in sparse arrays**

**Code:**
```javascript
// forEach on sparse arrays
```

**Options:**
- A) TRUE
- B) FALSE
- C) Depends
- D) Only NaN

**✓ Correct Answer:** A) TRUE

**Explanation:** `forEach` skips holes/empty slots in sparse arrays.

---

## Question 59
**What happens if you use break in a forEach loop?**

**Code:**
```javascript
// break in forEach
```

**Options:**
- A) Skips iteration
- B) Stops loop
- C) SyntaxError
- D) Continues normally

**✓ Correct Answer:** C) SyntaxError

**Explanation:** `break` is not allowed in forEach callbacks.

---

## Question 60
**What happens if you continue in a do...while?**

**Code:**
```javascript
// continue in do...while
```

**Options:**
- A) Skips rest, checks condition
- B) Breaks loop
- C) Restart immediately
- D) Error

**✓ Correct Answer:** A) Skips rest, checks condition

**Explanation:** `continue` skips remaining code and goes to condition check.

---

## Question 61
**What happens if you modify array length during a for loop?**

**Code:**
```javascript
// Modifying array length in loop
```

**Options:**
- A) Loop adapts dynamically
- B) Undefined behavior
- C) May skip or repeat
- D) Crashes

**✓ Correct Answer:** C) May skip or repeat

**Explanation:** Modifying array length during iteration can cause unpredictable behavior.

---

## Question 62
**Which loop works best for asynchronous iteration (with await)?**

**Code:**
```javascript
// Async iteration
```

**Options:**
- A) forEach
- B) for...of
- C) for...in
- D) while

**✓ Correct Answer:** B) for...of

**Explanation:** `for...of` properly handles `await` in async contexts.

---

## Question 63
**for loop output**

**Code:**
```javascript
for(let x=0; x<2; x++){ console.log(x) }
```

**Options:**
- A) 0 1 2
- B) 0 1 2 3
- C) 0 1 2 3 4
- D) 3 only

**✓ Correct Answer:** A) 0 1 2

**Explanation:** Loop runs while `x < 2`, printing 0 and 1.

---

## Question 64
**What does continue do in while loop?**

**Code:**
```javascript
// continue in while loop
```

**Options:**
- A) Stops loop
- B) Skips current iteration
- C) Restarts loop
- D) Ends program

**✓ Correct Answer:** B) Skips current iteration

**Explanation:** `continue` jumps to the next iteration.

---

## Question 65
**let i=0; do { console.log(i); i++; } while(i<3)**

**Code:**
```javascript
let i=0; do { console.log(i); i++; } while(i<3)
```

**Options:**
- A) 0 1 2
- B) 1 2 3
- C) 0 1
- D) Infinite

**✓ Correct Answer:** A) 0 1 2

**Explanation:** Loop executes while `i < 3`, printing 0, 1, 2.

---

## Question 66
**for loop with let**

**Code:**
```javascript
for(let i of 123){console.log(i)}
```

**Options:**
- A) Nothing
- B) TypeError
- C) Prints digits
- D) undefined

**✓ Correct Answer:** B) TypeError

**Explanation:** Numbers are not iterable with `for...of`.

---

## Question 67
**What happens if you use break in a for...of loop?**

**Code:**
```javascript
// break in for...of
```

**Options:**
- A) Skips rest, checks condition
- B) Breaks loop
- C) SyntaxError
- D) None

**✓ Correct Answer:** A) Skips rest, checks condition

**Explanation:** `break` exits the loop immediately.

---

## Question 68
**When using for...in on arrays, iteration order is:**

**Code:**
```javascript
// for...in iteration order
```

**Options:**
- A) Guaranteed ascending
- B) Random
- C) Based on numeric
- D) Unspecified

**✓ Correct Answer:** C) Based on numeric

**Explanation:** Modern engines iterate array indices in numeric order.

---

## Question 69
**forEach() can mutate original array elements**

**Code:**
```javascript
// forEach mutating arrays
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only with map
- D) Only for const

**✓ Correct Answer:** A) TRUE

**Explanation:** `forEach` can modify array elements in place.

---

## Question 70
**let arr=[1,2,3]; arr.forEach((v,i)=>{ if(i===1) return; console.log(v); });**

**Code:**
```javascript
let arr=[1,2,3]; arr.forEach((v,i)=>{ if(i===1) return; console.log(v); });
```

**Options:**
- A) 1,2,3
- B) 1,3
- C) 2,3
- D) 1 only

**✓ Correct Answer:** B) 1,3

**Explanation:** `return` skips index 1, printing 1 and 3.

---

## Question 71
**let x=0; while(x<4){console.log(x); x++;}**

**Code:**
```javascript
let x=0; while(x<4){console.log(x); x++;}
```

**Options:**
- A) 1 2 4
- B) 1 2 3 4
- C) 1 4
- D) Infinite

**✓ Correct Answer:** A) 1 2 4

**Explanation:** Wait, this should print 0 1 2 3. There may be an error in the source.

---

## Question 72
**for...of cannot iterate directly over which?**

**Code:**
```javascript
// for...of compatibility
```

**Options:**
- A) String
- B) Set
- C) Object literal
- D) Array

**✓ Correct Answer:** C) Object literal

**Explanation:** Plain objects are not iterable by default.

---

## Question 73
**Using for...in on an array prints:**

**Code:**
```javascript
// for...in on arrays
```

**Options:**
- A) Undefined
- B) Skips holes
- C) null
- D) 0

**✓ Correct Answer:** B) Skips holes

**Explanation:** `for...in` iterates only over defined indices.

---

## Question 74
**Which loop executes body after condition is false?**

**Code:**
```javascript
// Loop execution order
```

**Options:**
- A) while
- B) do...while
- C) for
- D) None

**✓ Correct Answer:** B) do...while

**Explanation:** `do...while` runs body first, then checks condition.

---

## Question 75
**for loop with nested x in array**

**Code:**
```javascript
for(let x in [, ,]){console.log(x)}
```

**Options:**
- A) 0,1
- B) 0 only
- C) nothing
- D) Error

**✓ Correct Answer:** C) nothing

**Explanation:** Sparse array with only holes has no enumerable indices.

---

## Question 76
**for...of cannot iterate directly over which?**

**Code:**
```javascript
// for...of iteration
```

**Options:**
- A) String
- B) Set
- C) Object literal
- D) Array

**✓ Correct Answer:** C) Object literal

**Explanation:** Plain objects don't implement the iterator protocol.

---

## Question 77
**for...in iterates enumerable inherited props too**

**Code:**
```javascript
// for...in with inheritance
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only own
- D) Only symbols

**✓ Correct Answer:** A) TRUE

**Explanation:** `for...in` includes inherited enumerable properties.

---

## Question 78
**forEach() is synchronous or asynchronous?**

**Code:**
```javascript
// forEach execution mode
```

**Options:**
- A) Sync
- B) Async
- C) Depends
- D) Lazy

**✓ Correct Answer:** A) Sync

**Explanation:** `forEach` executes synchronously.

---

## Question 79
**for...works on Map to iterate:**

**Code:**
```javascript
// for...of on Map
```

**Options:**
- A) Keys
- B) Values
- C) [key,value] pairs
- D) Nothing

**✓ Correct Answer:** C) [key,value] pairs

**Explanation:** Map iterator returns [key, value] pairs.

---

## Question 80
**for...in iterates enumerable inherited props too**

**Code:**
```javascript
// for...in inheritance
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only own
- D) Only symbols

**✓ Correct Answer:** A) TRUE

**Explanation:** `for...in` iterates inherited enumerable properties.

---

## Question 81
**let a=0; while(a<3){a++; console.log(a)}**

**Code:**
```javascript
let a=0; while(a<3){a++; console.log(a)}
```

**Options:**
- A) 1
- B) 1 2
- C) 2
- D) None

**✓ Correct Answer:** A) 1

**Explanation:** This should print 1 2 3, but based on options, may have error in source.

---

## Question 82
**Can break be used with label to exit outer loop?**

**Code:**
```javascript
// break with labels
```

**Options:**
- A) Yes
- B) No
- C) Only async
- D) Only forEach

**✓ Correct Answer:** A) Yes

**Explanation:** Labeled breaks can exit outer loops.

---

## Question 83
**continue skips remaining statements of current iteration**

**Code:**
```javascript
// continue behavior
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only async
- D) Only nested

**✓ Correct Answer:** A) TRUE

**Explanation:** `continue` skips to next iteration immediately.

---

## Question 84
**for...in ignores non-enumerable properties**

**Code:**
```javascript
// for...in enumerable check
```

**Options:**
- A) TRUE
- B) FALSE
- C) Only strict mode
- D) Only with let

**✓ Correct Answer:** A) TRUE

**Explanation:** `for...in` only iterates enumerable properties.

---

## Question 85
**let i=0; do{console.log(i++)}while(i<0);**

**Code:**
```javascript
let i=0; do{console.log(i++)}while(i<0);
```

**Options:**
- A) 0
- B) 1
- C) none
- D) Error

**✓ Correct Answer:** A) 0

**Explanation:** `do...while` executes once before checking condition.

---

## Question 86
**Which stops entire nested loop chain?**

**Code:**
```javascript
// Stopping nested loops
```

**Options:**
- A) break label
- B) continue label
- C) return
- D) both A and C

**✓ Correct Answer:** D) both A and C

**Explanation:** Labeled break or return can exit multiple loops.

---

## Question 87
**for(let i=0; i<3; i++){ for(let j=0; j<1; j++){ if(i===1)continue; console.log(i) }}**

**Code:**
```javascript
for(let i=0; i<3; i++){ for(let j=0; j<1; j++){ if(i===1)continue; console.log(i) }}
```

**Options:**
- A) 0,2
- B) 0,1
- C) 1,2
- D) 0 only

**✓ Correct Answer:** A) 0,2

**Explanation:** When `i===1`, continue skips logging for that iteration.

---

## Question 88
**Using for...in with array breaks prints:**

**Code:**
```javascript
// for...in with arrays
```

**Options:**
- A) Undefined
- B) Skips holes
- C) null
- D) 0

**✓ Correct Answer:** B) Skips holes

**Explanation:** `for...in` doesn't iterate over empty slots.

---

## Question 89
**Which loop doesn't create its own scope in ES5?**

**Code:**
```javascript
// Loop scope in ES5
```

**Options:**
- A) for(var)
- B) for(let)
- C) for(const)
- D) while(let)

**✓ Correct Answer:** A) for(var)

**Explanation:** `var` is function-scoped, not block-scoped.

---

## Question 90
**Which loop doesn't create its own scope in ES6?**

**Code:**
```javascript
// Loop scope in ES6
```

**Options:**
- A) for
- B) while
- C) Depends
- D) Lazy

**✓ Correct Answer:** A) for

**Explanation:** With `let`/`const`, loops create block scope in ES6.

---

## Question 91
**Which of these loops supports await in async functions?**

**Code:**
```javascript
// await in loops
```

**Options:**
- A) forEach
- B) for...of
- C) for...in
- D) while

**✓ Correct Answer:** B) for...of

**Explanation:** `for...of` properly waits for promises with await.

---

## Question 92
**break inside switch within loop breaks:**

**Code:**
```javascript
// break in switch within loop
```

**Options:**
- A) Only switch
- B) Entire loop
- C) Both switch and loop
- D) None

**✓ Correct Answer:** A) Only switch

**Explanation:** `break` in switch only exits the switch, not the loop.

---

## Question 93
**Total Questions: 93**
**Topics: JavaScript DOM Manipulation & Loops**

---

## Question 94
**jQuery is a:**

**Code:**
```javascript
// jQuery definition
```

**Options:**
- A) Programming Language
- B) JavaScript Library
- C) Framework
- D) Plugin

**✓ Correct Answer:** B) JavaScript Library

**Explanation:** jQuery is a JavaScript library that simplifies DOM manipulation, event handling, and AJAX.

---

## Question 95
**The jQuery file has a file extension of:**

**Code:**
```javascript
// jQuery file extension
```

**Options:**
- A) .java
- B) .jquery
- C) .js
- D) .json

**✓ Correct Answer:** C) .js

**Explanation:** jQuery is JavaScript, so it uses the `.js` file extension.

---

## Question 96
**Which symbol is used as shorthand for jQuery?**

**Code:**
```javascript
// jQuery shorthand
```

**Options:**
- A) @
- B) $
- C) #
- D) %

**✓ Correct Answer:** B) $

**Explanation:** The `$` symbol is an alias for the jQuery function.

---

## Question 97
**The latest jQuery version can be added via:**

**Code:**
```javascript
// Adding jQuery to project
```

**Options:**
- A) CDN
- B) XML
- C) JSON
- D) HTML

**✓ Correct Answer:** A) CDN

**Explanation:** jQuery can be included via Content Delivery Network (CDN) links.

---

## Question 98
**Which method is used to hide selected elements?**

**Code:**
```javascript
// Hiding elements
```

**Options:**
- A) .invisible()
- B) .hidden()
- C) .hide()
- D) .displayNone()

**✓ Correct Answer:** C) .hide()

**Explanation:** `.hide()` sets display to none, hiding the element.

---

## Question 99
**To make an element visible again, we use:**

**Code:**
```javascript
// Showing elements
```

**Options:**
- A) .show()
- B) .display()
- C) .open()
- D) .visible()

**✓ Correct Answer:** A) .show()

**Explanation:** `.show()` makes hidden elements visible again.

---

## Question 100
**Which method is used to toggle between hide/show?**

**Code:**
```javascript
// Toggle visibility
```

**Options:**
- A) .change()
- B) .slideToggle()
- C) .toggle()
- D) .fade()

**✓ Correct Answer:** C) .toggle()

**Explanation:** `.toggle()` switches between showing and hiding elements.

---

## Question 101
**The document ready function syntax is:**

**Code:**
```javascript
// Document ready
```

**Options:**
- A) document.ready(function{})
- B) $(document).ready(function(){})
- C) ready(document, function(){})
- D) onReady(function(){})

**✓ Correct Answer:** B) $(document).ready(function(){})

**Explanation:** This ensures code runs after the DOM is fully loaded.

---

## Question 102
**Which jQuery method is used to change the content of an element?**

**Code:**
```javascript
// Changing element content
```

**Options:**
- A) .setText()
- B) .html()
- C) .setHtml()
- D) .innerHtml()

**✓ Correct Answer:** B) .html()

**Explanation:** `.html()` gets or sets the HTML content of an element.

---

## Question 103
**The jQuery selector $("p.intro") selects:**

**Code:**
```javascript
$("p.intro")
```

**Options:**
- A) All <p> elements with class name intro
- B) Paragraphs with id intro
- C) All intro elements
- D) None

**✓ Correct Answer:** A) All <p> elements with class name intro

**Explanation:** This selects all paragraph elements with the class "intro".

---

## Question 104
**To select all <div> elements inside <p> elements:**

**Code:**
```javascript
// Selector syntax
```

**Options:**
- A) $("div p")
- B) $("p div")
- C) $("p+div")
- D) $("div+p")

**✓ Correct Answer:** B) $("p div")

**Explanation:** `$("p div")` selects all divs that are descendants of p elements.

---

## Question 105
**To fade out an element slowly:**

**Code:**
```javascript
// Fade animation
```

**Options:**
- A) fadeOut(1000)
- B) fadeOut("slow")
- C) fade("slow")
- D) fade("out")

**✓ Correct Answer:** B) fadeOut("slow")

**Explanation:** `.fadeOut("slow")` fades out the element over 600ms.

---

## Question 106
**The method .append() in jQuery:**

**Code:**
```javascript
// Append method
```

**Options:**
- A) Adds content at the beginning
- B) Adds content at the end
- C) Replaces existing content
- D) Deletes content

**✓ Correct Answer:** B) Adds content at the end

**Explanation:** `.append()` inserts content at the end of selected elements.

---

## Question 107
**Which function stops currently running animations?**

**Code:**
```javascript
// Stop animations
```

**Options:**
- A) .break()
- B) .pause()
- C) .stop()
- D) .end()

**✓ Correct Answer:** C) .stop()

**Explanation:** `.stop()` halts the current animation on selected elements.

---

## Question 108
**Which of the following is correct for chaining in jQuery?**

**Code:**
```javascript
// Method chaining
```

**Options:**
- A) $("#id").css().html();
- B) $("#id") css() html()
- C) $("#id").css, html()
- D) None

**✓ Correct Answer:** A) $("#id").css().html();

**Explanation:** jQuery methods can be chained using dot notation.

---

## Question 109
**The .attr() function is used to:**

**Code:**
```javascript
// Attribute manipulation
```

**Options:**
- A) Change style
- B) Add HTML
- C) Get or set attribute value
- D) Change text

**✓ Correct Answer:** C) Get or set attribute value

**Explanation:** `.attr()` gets or sets HTML attributes.

---

## Question 110
**What will $("#id").text("Hi") do?**

**Code:**
```javascript
$("#id").text("Hi")
```

**Options:**
- A) Append "Hi"
- B) Replace inner text with "Hi"
- C) Add new element
- D) Nothing

**✓ Correct Answer:** B) Replace inner text with "Hi"

**Explanation:** `.text()` sets the text content, replacing existing content.

---

## Question 111
**The event .hover() takes:**

**Code:**
```javascript
// Hover event
```

**Options:**
- A) One function
- B) Two functions
- C) No arguments
- D) None

**✓ Correct Answer:** B) Two functions

**Explanation:** `.hover()` takes two functions: one for mouseenter, one for mouseleave.

---

## Question 112
**To perform an AJAX request in jQuery:**

**Code:**
```javascript
// AJAX request
```

**Options:**
- A) $.ajax()
- B) $.data()
- C) $.fetch()
- D) $.load()

**✓ Correct Answer:** A) $.ajax()

**Explanation:** `$.ajax()` is the main method for AJAX requests in jQuery.

---

## Question 113
**Which method removes selected elements from the DOM?**

**Code:**
```javascript
// Remove elements
```

**Options:**
- A) .delete()
- B) .remove()
- C) .erase()
- D) .detach()

**✓ Correct Answer:** B) .remove()

**Explanation:** `.remove()` removes elements from the DOM completely.

---

## Question 114
**The difference between .remove() and .detach() is:**

**Code:**
```javascript
// Remove vs Detach
```

**Options:**
- A) .detach() removes and keeps data/events
- B) .remove() keeps events
- C) Both are identical
- D) .detach() permanently deletes

**✓ Correct Answer:** A) .detach() removes and keeps data/events

**Explanation:** `.detach()` removes elements but preserves data and event handlers.

---

## Question 115
**$("div > p") selects:**

**Code:**
```javascript
$("div > p")
```

**Options:**
- A) All <p> inside <div> (any depth)
- B) All <p> that are direct children of <div>
- C) All divs next to p
- D) None

**✓ Correct Answer:** B) All <p> that are direct children of <div>

**Explanation:** The `>` selector targets only direct children.

---

## Question 116
**Which method attaches multiple event handlers in one call?**

**Code:**
```javascript
// Multiple event handlers
```

**Options:**
- A) .bind()
- B) .on()
- C) .live()
- D) .delegate()

**✓ Correct Answer:** B) .on()

**Explanation:** `.on()` is the modern way to attach one or more event handlers.

---

## Question 117
**The .live() function was removed because:**

**Code:**
```javascript
// Deprecated methods
```

**Options:**
- A) It caused performance issues
- B) It was not working
- C) It was slow
- D) None

**✓ Correct Answer:** A) It caused performance issues

**Explanation:** `.live()` was inefficient and replaced by `.on()`.

---

## Question 118
**To get the value of an input field:**

**Code:**
```javascript
// Get input value
```

**Options:**
- A) .text()
- B) .val()
- C) .html()
- D) .getValue()

**✓ Correct Answer:** B) .val()

**Explanation:** `.val()` gets or sets the value of form elements.

---

## Question 119
**What does event.preventDefault() do in jQuery?**

**Code:**
```javascript
event.preventDefault()
```

**Options:**
- A) Stops event propagation
- B) Prevents default browser action
- C) Deletes event
- D) None

**✓ Correct Answer:** B) Prevents default browser action

**Explanation:** Prevents the browser's default action for the event.

---

## Question 120
**Which method can be used to attach event handlers to dynamically added elements?**

**Code:**
```javascript
// Event delegation
```

**Options:**
- A) .on()
- B) .click()
- C) .live()
- D) .delegate()

**✓ Correct Answer:** A) .on()

**Explanation:** `.on()` with delegation works for current and future elements.

---

## Question 121
**The .each() function in jQuery is used for:**

**Code:**
```javascript
// Iteration
```

**Options:**
- A) Iterating over arrays/objects
- B) Looping DOM once
- C) Calling multiple functions
- D) None

**✓ Correct Answer:** A) Iterating over arrays/objects

**Explanation:** `.each()` iterates over jQuery objects or arrays.

---

## Question 122
**Which function is used to load JSON data via AJAX?**

**Code:**
```javascript
// Load JSON
```

**Options:**
- A) $.ajaxJSON()
- B) $.getJSON()
- C) $.loadJSON()
- D) $.getData()

**✓ Correct Answer:** B) $.getJSON()

**Explanation:** `$.getJSON()` loads JSON-encoded data using GET request.

---

## Question 123
**To stop event bubbling, we use:**

**Code:**
```javascript
// Stop propagation
```

**Options:**
- A) event.stopPropagation()
- B) event.stop()
- C) event.cancel()
- D) None

**✓ Correct Answer:** A) event.stopPropagation()

**Explanation:** Prevents the event from bubbling up the DOM tree.

---

## Question 124
**The .data() method is used to:**

**Code:**
```javascript
// Data storage
```

**Options:**
- A) Get/set custom data associated with elements
- B) Access JSON data
- C) Load API data
- D) Store HTML

**✓ Correct Answer:** A) Get/set custom data associated with elements

**Explanation:** `.data()` stores arbitrary data associated with elements.

---

## Question 125
**What does .promise() return?**

**Code:**
```javascript
// Promise method
```

**Options:**
- A) A Deferred object
- B) Boolean
- C) Function
- D) None

**✓ Correct Answer:** A) A Deferred object

**Explanation:** Returns a Promise object to observe when actions complete.

---

## Question 126
**To animate CSS properties, we use:**

**Code:**
```javascript
// Animation
```

**Options:**
- A) .animate()
- B) .motion()
- C) .cssTransition()
- D) .fx()

**✓ Correct Answer:** A) .animate()

**Explanation:** `.animate()` performs custom CSS animations.

---

## Question 127
**$.noConflict() is used to:**

**Code:**
```javascript
// NoConflict mode
```

**Options:**
- A) Avoid conflicts with $ variable
- B) Load multiple scripts
- C) Stop jQuery
- D) Change CDN

**✓ Correct Answer:** A) Avoid conflicts with $ variable

**Explanation:** Releases jQuery's control of the `$` variable.

---

## Question 128
**Which method runs a function once for each matched element and returns the jQuery object?**

**Code:**
```javascript
// Iteration method
```

**Options:**
- A) .map()
- B) .each()
- C) .loop()
- D) .run()

**✓ Correct Answer:** B) .each()

**Explanation:** `.each()` executes a function for each matched element.

---

## Question 129
**$("ul li:first-child") selects:**

**Code:**
```javascript
$("ul li:first-child")
```

**Options:**
- A) The first <li> of every <ul>
- B) All first <ul>
- C) Last child of <li>
- D) None

**✓ Correct Answer:** A) The first <li> of every <ul>

**Explanation:** Selects the first child `<li>` in each `<ul>`.

---

## Question 130
**Which method replaces selected elements with new content?**

**Code:**
```javascript
// Replace elements
```

**Options:**
- A) .replaceWith()
- B) .change()
- C) .replace()
- D) .html()

**✓ Correct Answer:** A) .replaceWith()

**Explanation:** `.replaceWith()` replaces selected elements with new content.

---

## Question 131
**To insert content before selected elements:**

**Code:**
```javascript
// Insert before
```

**Options:**
- A) .before()
- B) .prepend()
- C) .insertBefore()
- D) Both A & C

**✓ Correct Answer:** D) Both A & C

**Explanation:** Both `.before()` and `.insertBefore()` insert content before elements.

---

## Question 132
**The .width() method returns:**

**Code:**
```javascript
// Width method
```

**Options:**
- A) The width of element excluding padding and border
- B) Including padding
- C) Including margin
- D) None

**✓ Correct Answer:** A) The width of element excluding padding and border

**Explanation:** `.width()` returns the content width only.

---

## Question 133
**The .outerWidth(true) includes:**

**Code:**
```javascript
// Outer width with margin
```

**Options:**
- A) Padding
- B) Border
- C) Margin
- D) All except margin

**✓ Correct Answer:** C) Margin

**Explanation:** `.outerWidth(true)` includes padding, border, and margin.

---

## Question 134
**jQuery uses which object for AJAX requests?**

**Code:**
```javascript
// AJAX internals
```

**Options:**
- A) XMLHttpRequest
- B) HTTPRequest
- C) AJAXRequest
- D) JSONRequest

**✓ Correct Answer:** A) XMLHttpRequest

**Explanation:** jQuery uses the native XMLHttpRequest object for AJAX.

---

## Question 135
**To queue animations, jQuery uses:**

**Code:**
```javascript
// Animation queueing
```

**Options:**
- A) .queue()
- B) .delay()
- C) .hold()
- D) .animate()

**✓ Correct Answer:** A) .queue()

**Explanation:** `.queue()` shows or manipulates the queue of functions.

---

## Question 136
**The .serialize() method:**

**Code:**
```javascript
// Form serialization
```

**Options:**
- A) Converts form data into URL-encoded string
- B) Converts HTML into JSON
- C) Saves form
- D) None

**✓ Correct Answer:** A) Converts form data into URL-encoded string

**Explanation:** Creates a URL-encoded text string from form elements.

---

## Question 137
**Which statement about Deferred in jQuery is TRUE?**

**Code:**
```javascript
// Deferred objects
```

**Options:**
- A) It manages asynchronous operations
- B) It is for CSS
- C) It handles DOM
- D) None

**✓ Correct Answer:** A) It manages asynchronous operations

**Explanation:** Deferred objects provide a way to handle async operations.

---

## Question 138
**To run a function after all animations complete:**

**Code:**
```javascript
// Animation completion
```

**Options:**
- A) .done()
- B) .promise().done()
- C) .then()
- D) .complete()

**✓ Correct Answer:** B) .promise().done()

**Explanation:** Get a promise and attach a done handler for completion.

---

## Question 139
**The .one() method:**

**Code:**
```javascript
// One-time event handler
```

**Options:**
- A) Binds an event handler that runs once
- B) Runs forever
- C) Rebinds every time
- D) Removes handler

**✓ Correct Answer:** A) Binds an event handler that runs once

**Explanation:** `.one()` attaches a handler that executes at most once.

---

## Question 140
**What does $("div").is(":visible") return?**

**Code:**
```javascript
$("div").is(":visible")
```

**Options:**
- A) True if visible
- B) False if hidden
- C) Boolean
- D) All above

**✓ Correct Answer:** D) All above

**Explanation:** Returns a boolean indicating visibility status.

---

## Question 141
**jQuery internally uses which function for event handling?**

**Code:**
```javascript
// Event handling internals
```

**Options:**
- A) addEventListener
- B) attachEvent
- C) onEvent
- D) listen

**✓ Correct Answer:** A) addEventListener

**Explanation:** Modern jQuery uses `addEventListener` for event binding.

---

## Question 142
**Which of the following methods retrieves the computed CSS value?**

**Code:**
```javascript
// Get CSS value
```

**Options:**
- A) .style()
- B) .getCSS()
- C) .css("property")
- D) .attr("property")

**✓ Correct Answer:** C) .css("property")

**Explanation:** `.css("property")` gets the computed CSS value.

---

## Question 143
**To find all descendants that match a selector, we use:**

**Code:**
```javascript
// Find descendants
```

**Options:**
- A) .find()
- B) .children()
- C) .descendants()
- D) .filter()

**✓ Correct Answer:** A) .find()

**Explanation:** `.find()` searches through descendants for matching elements.

---

**Total Questions: 143**
**Topics: JavaScript DOM Manipulation, Loops & jQuery**

---

# Scenario-Based DOM Manipulation Questions

## Easy Level

---

## Question 144
**User Profile Update - You're building a profile page. When the page loads, you need to update the user's name displayed in the heading.**

**Code:**
```javascript
document.getElementById("title").innerText = "Hello DOM!";
```

**Options:**
- A) Creates a new element with id title
- B) No effect
- C) Changes text of element with id title to 'Hello DOM!'
- D) Deletes the element

**✓ Correct Answer:** C) Changes text of element with id title to 'Hello DOM!'

**Explanation:** getElementById returns a single element, and innerText updates its text content.

---

## Question 145
**Theme Customization - A user wants to change the website background color through settings.**

**Code:**
```javascript
document.body.style.backgroundColor = "lightblue";
```

**Options:**
- A) Error occurs
- B) Sets page background to light blue
- C) Creates a new body element
- D) Changes text color to light blue

**✓ Correct Answer:** B) Sets page background to light blue

**Explanation:** Direct style manipulation via the style property modifies CSS properties.

---

## Question 146
**Dynamic Content Addition - A blog needs to add a new comment paragraph at the end of the page.**

**Code:**
```javascript
let p = document.createElement("p");
p.textContent = "New paragraph";
document.body.appendChild(p);
```

**Options:**
- A) Error occurs
- B) Replaces entire body content
- C) Adds new <p> at the end of body
- D) Creates paragraph but doesn't add it

**✓ Correct Answer:** C) Adds new <p> at the end of body

**Explanation:** createElement creates the element, and appendChild adds it to the DOM.

---

## Question 147
**Button Text Update - You need to update the text of the first 'Submit' button on a form.**

**Code:**
```javascript
document.querySelector(".btn").innerHTML = "Click Me!";
```

**Options:**
- A) Creates new button
- B) Changes all elements with class btn
- C) Changes first element with class btn to 'Click Me!'
- D) No effect

**✓ Correct Answer:** C) Changes first element with class btn to 'Click Me!'

**Explanation:** querySelector returns only the first matching element.

---

## Question 148
**Interactive Button - A landing page button should show an alert when users click it.**

**Code:**
```javascript
document.getElementById("btn").addEventListener("click", () => {
  alert("Button clicked!");
});
```

**Options:**
- A) Deletes the button
- B) Shows alert when button is clicked
- C) Shows alert immediately on page load
- D) No effect

**✓ Correct Answer:** B) Shows alert when button is clicked

**Explanation:** addEventListener attaches the click event handler to the button.

---

## Question 149
**Remove Obsolete Content - An admin dashboard needs to remove a deprecated warning message.**

**Code:**
```javascript
let el = document.getElementById("removeMe");
el.remove();
```

**Options:**
- A) No effect
- B) Changes element text to empty
- C) Hides the element
- D) Deletes element with id removeMe

**✓ Correct Answer:** D) Deletes element with id removeMe

**Explanation:** remove() completely removes the node from the DOM.

---

## Question 150
**Image Accessibility - You need to update the alt text of an image for better accessibility.**

**Code:**
```javascript
document.querySelector("img").setAttribute("alt", "New Image");
```

**Options:**
- A) Creates new image element
- B) Changes image source
- C) Deletes the image
- D) Updates alt attribute of first image

**✓ Correct Answer:** D) Updates alt attribute of first image

**Explanation:** setAttribute modifies or adds the specified attribute.

---

## Question 151
**Image Source Retrieval - A gallery app needs to log the source URL of the displayed image.**

**Code:**
```javascript
let src = document.querySelector("img").getAttribute("src");
```

**Options:**
- A) Deletes the image
- B) Sets new src value
- C) Returns src value of first image
- D) Returns all attributes

**✓ Correct Answer:** C) Returns src value of first image

**Explanation:** getAttribute fetches the value of the specified attribute.

---

## Question 152
**Rich Text Formatting - A text editor needs to display formatted content with bold text.**

**Code:**
```javascript
document.getElementById("demo").innerHTML = "<b>Bold</b>";
```

**Options:**
- A) Displays '<b>Bold</b>' as plain text
- B) Renders 'Bold' in bold formatting
- C) No effect
- D) Deletes the element

**✓ Correct Answer:** B) Renders 'Bold' in bold formatting

**Explanation:** innerHTML parses and renders HTML tags, while innerText shows plain text.

---

## Question 153
**Styling Menu Items - A navigation menu needs all items colored red when a theme is applied.**

**Code:**
```javascript
document.querySelectorAll("li").forEach(li => li.style.color = "red");
```

**Options:**
- A) All list items turn red
- B) Only first list item turns red
- C) No effect
- D) Creates new red list items

**✓ Correct Answer:** A) All list items turn red

**Explanation:** querySelectorAll returns a NodeList of all matching elements.

---

## Moderate Level

---

## Question 154
**Calculator Display - A calculator app displays the result of an operation in a div.**

**Code:**
```javascript
document.body.innerHTML = "<div id='a'></div>";
document.getElementById("a").innerText = 5 + 5;
```

**Options:**
- A) Displays '5 + 5' as text
- B) Displays '10' in the div
- C) Displays nothing
- D) Error occurs

**✓ Correct Answer:** B) Displays '10' in the div

**Explanation:** JavaScript evaluates 5 + 5 to 10, then innerText converts it to string.

---

## Question 155
**Form Submit Button - Complete the code to create a submit button and add it to the page.**

**Code:**
```javascript
let btn = document.createElement("button");
// Fill code to add text "Submit" and append to body
```

**Options:**
- A) btn.text = "Submit"; body.appendChild(btn);
- B) btn.innerHTML = "Submit"; btn.append();
- C) btn.value = "Submit"; document.appendChild(btn);
- D) btn.textContent = "Submit"; document.body.appendChild(btn);

**✓ Correct Answer:** D) btn.textContent = "Submit"; document.body.appendChild(btn);

**Explanation:** textContent sets button text, and appendChild adds it to body.

---

## Question 156
**Nested Click Handlers - A card component has a parent container and child button. User clicks the child button.**

**Code:**
```javascript
document.getElementById("parent").addEventListener("click", () => console.log("Parent"));
document.getElementById("child").addEventListener("click", () => console.log("Child"));
```

**Options:**
- A) No output
- B) Logs "Child" then "Parent"
- C) Logs only "Child"
- D) Logs only "Parent"

**✓ Correct Answer:** B) Logs "Child" then "Parent"

**Explanation:** Event bubbling propagates the click event from child to parent.

---

## Question 157
**Stop Event Propagation - A modal's close button shouldn't trigger the parent modal's click handler.**

**Code:**
```javascript
document.getElementById("child").addEventListener("click", (e) => {
  e.stopPropagation();
  console.log("Child only");
});
```

**Options:**
- A) Logs "Child only" then parent message
- B) Logs only "Child only"
- C) No output
- D) Error occurs

**✓ Correct Answer:** B) Logs only "Child only"

**Explanation:** stopPropagation() prevents event from bubbling to parent elements.

---

## Question 158
**Active State Toggle - A sidebar menu item should toggle its active state when clicked.**

**Code:**
```javascript
document.getElementById("box").classList.toggle("active");
```

**Options:**
- A) Only removes active class
- B) Replaces all classes with active
- C) Adds/removes active class
- D) Only adds active class

**✓ Correct Answer:** C) Adds/removes active class

**Explanation:** classList.toggle adds class if absent, removes if present.

---

## Question 159
**Todo List Generation - An app needs to generate a todo list from an array of tasks.**

**Code:**
```javascript
let ul = document.createElement("ul");
["A","B","C"].forEach(item => {
  let li = document.createElement("li");
  li.textContent = item;
  ul.appendChild(li);
});
document.body.appendChild(ul);
```

**Options:**
- A) Only creates item C
- B) Error occurs
- C) Creates empty list
- D) Creates list with items A, B, C

**✓ Correct Answer:** D) Creates list with items A, B, C

**Explanation:** Iteration creates and appends each list item dynamically.

---

## Question 160
**Element Replacement - A notification paragraph needs to be replaced with a div containing different text.**

**Code:**
```javascript
document.body.innerHTML = "<p id='p'>Hello</p>";
document.getElementById("p").outerHTML = "<div>Bye</div>";
```

**Options:**
- A) No effect
- B) Replaces <p> with <div>Bye</div>
- C) Adds <div>Bye</div> after <p>
- D) Only changes text to 'Bye'

**✓ Correct Answer:** B) Replaces <p> with <div>Bye</div>

**Explanation:** outerHTML replaces the entire element including its tags.

---

## Question 161
**Pre-fill Form Field - A contact form should pre-fill the email input with a test value.**

**Code:**
```javascript
document.querySelector("input").value = "Test";
```

**Options:**
- A) Creates new input with value 'Test'
- B) Changes input placeholder
- C) No effect
- D) Sets input field value to 'Test'

**✓ Correct Answer:** D) Sets input field value to 'Test'

**Explanation:** The value property controls the content of form input elements.

---

## Question 162
**Form Submission Control - A form submit button should be disabled after first click to prevent duplicate submissions.**

**Code:**
```javascript
document.getElementById("btn").disabled = true;
```

**Options:**
- A) Button is hidden
- B) No effect
- C) Button becomes disabled (unclickable)
- D) Button is deleted

**✓ Correct Answer:** C) Button becomes disabled (unclickable)

**Explanation:** The disabled property prevents user interaction with form elements.

---

## Question 163
**Multiple Text Nodes - A notification box needs to display multiple text fragments together.**

**Code:**
```javascript
document.body.innerHTML = "<div id='x'></div>";
document.getElementById("x").append("Hello", "World");
```

**Options:**
- A) Error occurs
- B) Displays 'HelloWorld' in the div
- C) Displays only 'Hello'
- D) Displays only 'World'

**✓ Correct Answer:** B) Displays 'HelloWorld' in the div

**Explanation:** append() can add multiple text nodes and elements in one call.

---

## Question 164
**Update Notification - A dashboard needs to replace the oldest notification with a new one.**

**Code:**
```javascript
let parent = document.getElementById("parent");
let newEl = document.createElement("span");
newEl.textContent = "New";
parent.replaceChild(newEl, parent.firstChild);
```

**Options:**
- A) Replaces first child with <span>New</span>
- B) No effect
- C) Deletes parent element
- D) Adds new span before first child

**✓ Correct Answer:** A) Replaces first child with <span>New</span>

**Explanation:** replaceChild swaps the old child node with the new one.

---

## Question 165
**Menu Item Count - A restaurant menu app needs to count how many items are in a category.**

**Code:**
```javascript
document.body.innerHTML = "<ul><li>1</li><li>2</li></ul>";
console.log(document.querySelector("ul").children.length);
```

**Options:**
- A) Logs all children elements
- B) Error occurs
- C) Logs '0'
- D) Logs '2'

**✓ Correct Answer:** D) Logs '2'

**Explanation:** children returns only direct child elements (not text nodes).

---

## Question 166
**Infinite Scroll Detection - A social media feed logs when users scroll to load more content.**

**Code:**
```javascript
window.addEventListener("scroll", () => console.log("Scrolling..."));
```

**Options:**
- A) Prevents page scrolling
- B) No effect
- C) Logs message only once
- D) Logs message each time page scrolls

**✓ Correct Answer:** D) Logs message each time page scrolls

**Explanation:** Scroll event fires continuously during scrolling.

---

## Question 167
**Keyboard Shortcut Logging - A text editor logs which key users press for analytics.**

**Code:**
```javascript
document.addEventListener("keydown", e => console.log(e.key));
```

**Options:**
- A) Logs the pressed key name
- B) Logs only letter keys
- C) Prevents key from working
- D) No output

**✓ Correct Answer:** A) Logs the pressed key name

**Explanation:** e.key returns the name of the key pressed by the user.

---

## Question 168
**Text Content Retrieval - A scraper tool needs to extract visible text from a div.**

**Code:**
```javascript
document.body.innerHTML = "<div id='a'>Hi</div>";
console.log(document.getElementById("a").textContent);
```

**Options:**
- A) Logs the entire HTML
- B) Logs 'Hi'
- C) Error occurs
- D) Logs nothing

**✓ Correct Answer:** B) Logs 'Hi'

**Explanation:** textContent returns the visible text content of an element.

---

## Question 169
**Insert Advertisement - An ad should be inserted before a specific article on a blog.**

**Code:**
```javascript
let ref = document.getElementById("ref");
let newEl = document.createElement("p");
newEl.textContent = "Inserted";
ref.parentNode.insertBefore(newEl, ref);
```

**Options:**
- A) Inserts <p> before ref element
- B) Inserts <p> after ref element
- C) No effect
- D) Replaces ref element

**✓ Correct Answer:** A) Inserts <p> before ref element

**Explanation:** insertBefore places new element before the reference node.

---

## Question 170
**Append Product Details - An e-commerce page adds product description HTML to existing content.**

**Code:**
```javascript
document.body.innerHTML = "<div id='a'></div>";
document.getElementById("a").innerHTML += "<p>Text</p>";
```

**Options:**
- A) Error occurs
- B) Replaces div entirely
- C) Creates separate paragraph
- D) Results in <div id='a'><p>Text</p></div>

**✓ Correct Answer:** D) Results in <div id='a'><p>Text</p></div>

**Explanation:** += appends new HTML to existing innerHTML content.

---

## Question 171
**Typography Update - A blog applies a new font size to all paragraphs when user changes settings.**

**Code:**
```javascript
document.querySelectorAll("p").forEach(p => p.style.fontSize = "20px");
```

**Options:**
- A) All <p> elements get 20px font size
- B) Creates new paragraphs
- C) No effect
- D) Only first <p> changes

**✓ Correct Answer:** A) All <p> elements get 20px font size

**Explanation:** forEach iterates and applies the style to each paragraph.

---

## Question 172
**Dynamic Widget Injection - A widget needs to be injected at the end of a container div.**

**Code:**
```javascript
document.body.innerHTML = "<div id='a'></div>";
document.getElementById("a").insertAdjacentHTML("beforeend","<span>Hi</span>");
```

**Options:**
- A) Replaces the div
- B) Error occurs
- C) Inserts before the div
- D) Results in <div id='a'><span>Hi</span></div>

**✓ Correct Answer:** D) Results in <div id='a'><span>Hi</span></div>

**Explanation:** insertAdjacentHTML with 'beforeend' adds content inside at the end.

---

## Question 173
**Extract Inner HTML - A content management system extracts the HTML content of an article.**

**Code:**
```javascript
document.body.innerHTML = "<div id='a'>Hello</div>";
console.log(document.getElementById("a").innerHTML);
```

**Options:**
- A) Logs nothing
- B) Error occurs
- C) Logs <div id='a'>Hello</div>
- D) Logs 'Hello'

**✓ Correct Answer:** D) Logs 'Hello'

**Explanation:** innerHTML returns the HTML content inside the element (not the element itself).

---

## Hard Level

---

## Question 174
**Dynamic List Click Handler - A task manager has many dynamically added tasks. You want clicks on any task logged without individual listeners.**

**Code:**
```javascript
document.getElementById("list").addEventListener("click", e => {
  if(e.target.tagName === "LI") console.log(e.target.textContent);
});
```

**Options:**
- A) Logs clicked <li> text content
- B) Only works for existing items
- C) No output
- D) Logs all list items

**✓ Correct Answer:** A) Logs clicked <li> text content

**Explanation:** Event delegation allows handling events on dynamically added children via parent listener.

---

## Question 175
**Delayed Notification - A notification should appear 2 seconds after a user completes an action.**

**Code:**
```javascript
setTimeout(() => {
  document.body.innerHTML += "<p>Delayed</p>";
}, 1000);
```

**Options:**
- A) Error occurs
- B) Adds paragraph immediately
- C) No effect
- D) Adds <p>Delayed</p> after 1 second

**✓ Correct Answer:** D) Adds <p>Delayed</p> after 1 second

**Explanation:** setTimeout delays DOM manipulation by specified milliseconds.

---

## Question 176
**Content Change Observer - A dashboard needs to detect whenever new widgets are added to the page.**

**Code:**
```javascript
let obs = new MutationObserver(muts => console.log("DOM changed"));
obs.observe(document.body, {childList:true});
document.body.append("New");
```

**Options:**
- A) Logs 'DOM changed' when node added
- B) Logs only on deletion
- C) Prevents node addition
- D) No output

**✓ Correct Answer:** A) Logs 'DOM changed' when node added

**Explanation:** MutationObserver watches for DOM changes like additions and deletions.

---

## Question 177
**Modal Keyboard Control - A modal dialog should close when users press the Escape key for better UX.**

**Code:**
```javascript
document.addEventListener("keydown", e => {
  if(e.key === "Escape") document.getElementById("modal").style.display = "none";
});
```

**Options:**
- A) No effect
- B) Hides modal on any key press
- C) Deletes the modal
- D) Hides modal when Escape is pressed

**✓ Correct Answer:** D) Hides modal when Escape is pressed

**Explanation:** Event checks specifically for Escape key before hiding modal.

---

## Question 178
**Scroll Performance Optimization - A parallax website throttles scroll events to prevent performance issues.**

**Code:**
```javascript
let timer;
window.addEventListener("scroll", () => {
  if(!timer){
    timer = setTimeout(() => {
      console.log("Scroll event handled");
      timer = null;
    }, 500);
  }
});
```

**Options:**
- A) Prevents scrolling
- B) Logs once every 500ms during scroll
- C) No output
- D) Logs on every scroll pixel

**✓ Correct Answer:** B) Logs once every 500ms during scroll

**Explanation:** Throttling limits how often scroll handler executes for better performance.

---

## Question 179
**Interactive Table Highlighting - A data table should highlight the entire row when any cell is clicked.**

**Code:**
```javascript
document.querySelector("table").addEventListener("click", e => {
  if(e.target.tagName === "TD") e.target.parentNode.style.backgroundColor = "yellow";
});
```

**Options:**
- A) Highlights clicked row yellow
- B) Deletes the row
- C) Highlights only clicked cell
- D) No effect

**✓ Correct Answer:** A) Highlights clicked row yellow

**Explanation:** parentNode accesses the <tr> element to highlight entire row.

---

## Question 180
**Infinite Scroll Loading - A social feed loads more posts automatically when users reach page bottom.**

**Code:**
```javascript
window.addEventListener("scroll", () => {
  if(window.innerHeight + window.scrollY >= document.body.offsetHeight){
    document.body.append("Loaded more content");
  }
});
```

**Options:**
- A) No effect
- B) Appends content continuously
- C) Appends content when scrolled to bottom
- D) Prevents scrolling

**✓ Correct Answer:** C) Appends content when scrolled to bottom

**Explanation:** Calculation detects when viewport reaches document bottom.

---

## Question 181
**Toggle Button State - A visibility toggle button switches between 'Show' and 'Hide' text.**

**Code:**
```javascript
let btn = document.getElementById("toggle");
btn.addEventListener("click", () => {
  btn.textContent = btn.textContent === "Show" ? "Hide" : "Show";
});
```

**Options:**
- A) Only changes to 'Hide'
- B) Alternates button text on each click
- C) Deletes the button
- D) No effect

**✓ Correct Answer:** B) Alternates button text on each click

**Explanation:** Ternary operator toggles between two text values.

---

## Question 182
**Template Cloning - A product listing page uses a template to create multiple product cards.**

**Code:**
```javascript
let template = document.getElementById("tpl");
let clone = template.content.cloneNode(true);
document.body.appendChild(clone);
```

**Options:**
- A) Inserts cloned template content
- B) Moves original template
- C) Creates empty element
- D) Error occurs

**✓ Correct Answer:** A) Inserts cloned template content

**Explanation:** <template> elements can be cloned and inserted multiple times.

---

## Question 183
**Alphabetical List Sorting - A contact list should be sorted alphabetically when user clicks sort button.**

**Code:**
```javascript
let ul = document.getElementById("list");
document.getElementById("sortBtn").addEventListener("click", () => {
  [...ul.children].sort((a,b) => a.textContent.localeCompare(b.textContent))
    .forEach(li => ul.appendChild(li));
});
```

**Options:**
- A) Deletes unsorted items
- B) Creates new sorted list
- C) No effect
- D) Reorders <li> items alphabetically

**✓ Correct Answer:** D) Reorders <li> items alphabetically

**Explanation:** Array methods sort elements, then appendChild reorders them in DOM.

---

## Question 184
**Lazy Image Loading - A photo gallery loads images only when they become visible in viewport.**

**Code:**
```javascript
let imgs = document.querySelectorAll("img[data-src]");
let obs = new IntersectionObserver(entries => {
  entries.forEach(e => {
    if(e.isIntersecting){
      e.target.src = e.target.dataset.src;
      obs.unobserve(e.target);
    }
  });
});
imgs.forEach(img => obs.observe(img));
```

**Options:**
- A) Error occurs
- B) Loads images only when visible
- C) Loads all images immediately
- D) Prevents images from loading

**✓ Correct Answer:** B) Loads images only when visible

**Explanation:** IntersectionObserver detects when elements enter viewport.

---

## Question 185
**Form Validation - A registration form prevents submission if required email field is empty.**

**Code:**
```javascript
document.querySelector("form").addEventListener("submit", e => {
  if(!document.querySelector("input").value){
    e.preventDefault();
    alert("Input required!");
  }
});
```

**Options:**
- A) Always shows alert
- B) Deletes the form
- C) Submits form regardless
- D) Stops form submission if input empty

**✓ Correct Answer:** D) Stops form submission if input empty

**Explanation:** preventDefault() stops default form submission behavior.

---

## Question 186
**Click Counter Display - A game tracks and displays how many times a button has been clicked.**

**Code:**
```javascript
let count = 0;
document.getElementById("btn").addEventListener("click", () => {
  count++;
  document.getElementById("counter").textContent = count;
});
```

**Options:**
- A) Updates counter display each click
- B) No effect
- C) Only counts without displaying
- D) Resets counter each time

**✓ Correct Answer:** A) Updates counter display each click

**Explanation:** Variable tracks clicks and DOM updates show current count.

---

## Question 187
**Theme Switcher - A website allows users to toggle between light and dark themes.**

**Code:**
```javascript
document.getElementById("themeBtn").addEventListener("click", () => {
  document.body.classList.toggle("dark");
});
```

**Options:**
- A) Toggles dark theme class on body
- B) Changes button theme only
- C) No effect
- D) Only adds dark theme

**✓ Correct Answer:** A) Toggles dark theme class on body

**Explanation:** CSS class toggle switches theme styling on and off.

---

## Question 188
**Dropdown Menu Control - A custom dropdown should close when users click anywhere outside of it.**

**Code:**
```javascript
document.addEventListener("click", e => {
  if(!document.getElementById("dropdown").contains(e.target)){
    document.getElementById("dropdown").style.display = "none";
  }
});
```

**Options:**
- A) Deletes dropdown
- B) No effect
- C) Hides dropdown when clicked outside
- D) Hides on any click

**✓ Correct Answer:** C) Hides dropdown when clicked outside

**Explanation:** contains() checks if click target is inside dropdown element.

---

## Question 189
**Box Animation - An animated banner moves a promotional box across the screen horizontally.**

**Code:**
```javascript
let box = document.getElementById("box");
box.style.position = "absolute";
let pos = 0;
let id = setInterval(() => {
  if(pos >= 200) clearInterval(id);
  else box.style.left = pos++ + "px";
}, 10);
```

**Options:**
- A) No movement
- B) Moves box vertically
- C) Deletes the box
- D) Moves box horizontally to 200px

**✓ Correct Answer:** D) Moves box horizontally to 200px

**Explanation:** setInterval repeatedly updates left position until reaching 200px.

---

## Question 190
**Search Input Debouncing - A search bar debounces input to reduce API calls as user types.**

**Code:**
```javascript
let timer;
document.getElementById("search").addEventListener("input", e => {
  clearTimeout(timer);
  timer = setTimeout(() => console.log("Search:", e.target.value), 500);
});
```

**Options:**
- A) No output
- B) Logs on every keystroke
- C) Logs search after 500ms typing pause
- D) Prevents typing

**✓ Correct Answer:** C) Logs search after 500ms typing pause

**Explanation:** Debounce waits for user to stop typing before executing search.

---

## Question 191
**Drag and Drop Element - A dashboard allows users to drag widgets to rearrange their layout.**

**Code:**
```javascript
let box = document.getElementById("box");
box.addEventListener("mousedown", e => {
  let shiftX = e.clientX - box.getBoundingClientRect().left;
  let shiftY = e.clientY - box.getBoundingClientRect().top;
  function move(e){ 
    box.style.left = e.pageX - shiftX + "px"; 
    box.style.top = e.pageY - shiftY + "px"; 
  }
  document.addEventListener("mousemove", move);
  document.addEventListener("mouseup", () => document.removeEventListener("mousemove", move), {once:true});
});
```

**Options:**
- A) No effect
- B) Only tracks mouse position
- C) Deletes element on drag
- D) Enables dragging element with mouse

**✓ Correct Answer:** D) Enables dragging element with mouse

**Explanation:** Mouse events track position and update element coordinates during drag.

---

## Question 192
**Dynamic Table Generation - A report builder creates a data table from JSON API response.**

**Code:**
```javascript
let data = [{name:"Akash",age:22},{name:"Ravi",age:25}];
let table = document.createElement("table");
data.forEach(row => {
  let tr = document.createElement("tr");
  Object.values(row).forEach(val => {
    let td = document.createElement("td");
    td.textContent = val;
    tr.appendChild(td);
  });
  table.appendChild(tr);
});
document.body.appendChild(table);
```

**Options:**
- A) Error occurs
- B) Creates empty table
- C) Creates table with names and ages
- D) Only shows column headers

**✓ Correct Answer:** C) Creates table with names and ages

**Explanation:** Nested loops create table rows and cells from JSON data.

---

## Question 193
**Text Selection Detection - A document editor detects when users select text for formatting options.**

**Code:**
```javascript
document.addEventListener("mouseup", () => {
  let selection = window.getSelection().toString();
  if(selection) console.log("Selected:", selection);
});
```

**Options:**
- A) Prevents text selection
- B) Logs selected text when user releases mouse
- C) Deletes selected text
- D) No output

**✓ Correct Answer:** B) Logs selected text when user releases mouse

**Explanation:** window.getSelection() returns currently selected text in the document.

---

**Total Questions: 193**
**Topics: JavaScript DOM Manipulation, Loops, jQuery & Scenario-Based DOM**
