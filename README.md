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

**Total Questions: 43**
**Topic: JavaScript DOM Manipulation**
