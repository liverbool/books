---
title: reactjs
---

# Draft

# คำนำ

## Todos
### - principal of a single source of truth is two-way binding

วีคแรกที่ผมเริ่มศึกษา React ผมก็รู้สึกชอบมันอย่างจริงจัง แม้จะเป็นแฟนของ AngularJs อยู่แล้วก็ตามที แต่ผมก็ชอบมันจนรู้สึกตื่นเต้นที่จะเขียนอะไรถึงมัน ผมอยากแบ่งปันบางอย่างที่ผมคิดว่าจะเป็นประโยชน์กับคนที่สนใจอยากจะเรียน React และในที่สุด อะไรที่ว่าก็คือหนังสือเล่มนี้

ผมตั้งใจที่จะวางเนื้อหาในหนังสือเล่มให้ให้เป็น 3 ส่วนใหญ่ๆ คือ
  - ความรู้พื้นฐานทั่วไป เพื่อปูพื้นฐานที่จำเป็น
  - ส่วนที่เป็นเนื้อหาเกี่ยวกับ React
  - และส่วนที่เป็นการเขียน React Application แบบใช้งานจริง

ผมเห็นว่าความรู้พื้นฐานเป็นสิ่งสำคัญมาก และเมื่อคุณอ่านไปถึงส่วนที่ 3 คือ การเขียน React Application หากติดขัดอะไร จะได้เปิดย้อนกลับมาทบทวนดูความรู้พื้นฐานได้ด้วย

ผมไม่นิยมการนำเสนอแบบเขียน application code ไปด้วย อธิบายพื้นฐานไปด้วย แน่นอนว่าผมต้องอธิบายการเขียน code แต่ละบันทัด ว่ามันทำงานอย่างไร แต่ขัดใจที่จะเอาพื้นฐานไปปนไว้กับการเขียน code จริง ผมว่าเราควรมีพื้นฐานก่อนที่จะลงมือจริง ไม่งั้นคุณก็จะแค่ทำๆ ตามผม เหมือนผมเมื่อก่อนที่เสียเวลาทำตามๆ คนอื่นอยู่หลายปี โดยมีความเข้าใจที่ลึกซึ้งน้อยมาก ฉะนั้นจึงไม่อยากให้คนอ่านข้ามบทที่ว่าด้วยความรู้พื้นฐานไป

หลายคนอาจจะใจร้อนและข้ามไปอ่านบทการเขียน code จริงเลย หรืออ่านบทที่ว่าด้วยพื้นฐานแบบลวกๆ ผมว่าลองเสียเวลอ่านซักหน่อยเถอะครับ แม้ว่าคุณอาจจะคิดว่าคุณรู้มันแล้วก็ตาม ถือว่าทบทวนความรู้เก่า

ผมพยายามจะเขียนอธิบายความเป็นมาเป็นไปของสิ่งต่างๆ ที่เกี่ยวข้องพอประมาณ เพื่อเป็นจุดเริ่มต้นของนักพัฒนาหน้าใหม่ด้วย โดยพยายามจะไม่ทำให้นักพัฒนาหน้าเก่าต้องรำคาญใจ *ซึ่งยอมรับว่าเป็นงานที่อาจจะยากกว่าการอธิบาย React ซะอีก ;)*

ผมมีประสบการณ์ทำงานกับโปรแกรมเมอร์มายาวนานสิบกว่าปี เจอบรรดาโปรแกรมเมอร์น้อยใหญ่หลากหลาย เก่งบ้างไม่เก่งบ้างปะปนกันไป สิ่งหนึ่งที่ผมมองเห็นโปรแกรมเมอร์ส่วนมากทำกันก็คือ *การสนุกกับการละเลยความรู้พื้นฐาน* อาจเพราะเห็นว่ามันเป็นเรื่องหมูๆ แต่นั่นแหละครับ เมื่อรากฐานเราไม่มั่นคง ผลงานของเราจะยั่งยืนได้อย่างไร

# หนังสือเล่มนี้เหมาะสำหรับใคร?

ผมยากจะกำหนดความต้องการเบื้องต้นของผู้อ่านซักหน่อยนะครับ ไม่งั้นเราคงพูดกันไม่รู้เรื่อง หรือยากที่จะเข้าใจกันแน่ๆ เอาเป็นว่าก่อนอื่น ผมจะคิดเอาเองว่าคุณมีความรู้เรื่องเหล่านี้มาก่อนบ้างแล้ว หรือถ้ายังไม่รู้ ผมแนะนำให้ลองศึกษามันก่อนนะครับ ในเล่มเราจะไม่ได้สอนสิ่งเหล่านี้

  - **JavaScript** เป็นสิ่งแรกที่เราต้องรู้ และต้องเคยเขียนมันมาบ้างแล้ว ไม่ว่าจะด้วยการเขียนเพียวๆ หรือการใช้ไลบรารี่ เช่น jQuery หรืออื่นๆ ก็ตาม ยิ่งถ้าเชี่ยวชาญมากๆ ยิ่งดี

  - **Html** อันนี้ใส่ไว้ให้ครบเฉยๆ นะครับ ถ้าคุณยังไม่รู้จัก html แนะนำให้โยนหนังสือเล่มนี้ทิ้งได้เลย ​!! *(สายไปซะแล้ว)* แต่ผมคิดว่าวางไว้และหยิบมันมาอ่านอีกที เมื่อคุณกลับไปศึกษา html มันมาแล้วดีกว่านะครับ

  - **CSS** คู่กับ html อาจจไม่ถึงขนาดว่า Basic เท่า html แต่ก็ควรรู้มาบ้าง คุณคงไม่อยากเขียน application แบบไม่มีสีสันสวยงามเอาซะเลยหรอกนะครับ

  - **MVC (Optional)** อันนี้คาดหวังว่า ถ้าผู้อ่านรู้จัก ก็จะเป็นการเริ่มต้นกันที่ยอดเยี่ยมมากๆ แต่ถ้ายังไม่รู้จักมาก่อนก็ไม่เป็นไรครับ เราจะมาทำความรู้จักกันในหนังสือเล่มนี้


# What you can expect

  - **JSX** Todo ...

  - **ES6/7** Todo ...

  - **MVC Architecture** Todo ...

  - **Flux Architecture** Todo ...

  - **Immutable** Todo ...

  - **Component** Todo ...

  - **React Application** Todo ...


# Section 1 : Back to School

การเขียน React ต้องมีความรู้พื้นฐานหลายอย่างพอสมควร แม้กระทั่งว่าคนที่มีประสบการณ์การเขียน code มาบ้างหรือมากแล้วก็ตามที กระนั้นก็อาจจะประสบปัญหาในการเริ่มต้นได้ เพราะ React มีแนวคิดใหม่ๆ (ที่ยอดเยี่ยม) หลายอย่าง ความสูงชันในการเรียนรู้ React จึงค่อนข้างลิบริ่วเลยทีเดียว

แต่ผมสัญญาว่า ถ้าคุณใช้เวลาอย่างจริงจังกับหนังสือเล่มนี้ มันจะช่วยลดความสูงชันนั้นลงอยากมาก

แต่ก่อนอื่น เรามาทบทวนความรู้เก่าๆ กันซักนิด มาเริ่มกันเลยครับ !!


>
>
> การไม่รู้อะไรเลย คือความโง่เขลา
> การรู้ว่าไม่มีอะไรเลย คือความรู้ที่แท้จริง
>
>


# Chapter 1 : Introducing to ES6

ถ้าคุณเริ่มเขียน React และกำลังพยายามหาดู code ตัวอย่างใน internet บางทีคุณอาจจะงงเป็นไก่ตาแตกว่านั่นมัน JavaScript หรืออะไรกัน? ผมมั่นใจว่าคุณคงไม่อยากเป็นไก่ซึ่งถูกทำให้ตาแตก นั่นจึงเป็นเหตุผลที่เราต้องมาทำความรู้จักกับ ES6 หรือ ECMAScript6 กันก่อน


## ES6 Historical

[ECMAScript][1] คือข้อกำหนดมาตรฐานภาษาสคริปต์ (Scripting-language Specification) ของบริษัท **Ecma International** JavaScript ก็เป็นหนึ่งในภาษาสคริปต์ที่กำหนดโดย ECMAScript เช่นกัน ([1997][2]) และมันก็ถูกพัฒนามาหลายเวอร์ชั่น

เดิมที คุณลักษณะพิเศษของ JavaScript (Characteristic) ซึ่งถือเป็นเสน่ห์มายาวนาน *(เป็นภาษาที่ผมเองชื่นชอบมากที่สุด)* คือการเป็นภาษาแบบ [​Prototype based][3], [Prototypal Inheritance][4], [Variable Hoisting][5] ในยุครุ่งเรืองของอินเตอร์เน็ต JavaScript เติบโตมาเหนียวแน่นพร้อมๆ Web Browser โดยยังคงรักษาพื้นฐานนี้เรื่อยมา

ECMAScript 2015 หรือเวอร์ชั่นที่ 6 ของ ECMAScript มีการปรับปรุงความสามารถแบบขนานใหญ่ แบ่งเป็น 2 ส่วนหลักๆ ดังนี้

  - **Syntax** รูปแบบคำสั่งต่างๆ เปลี่ยนไปมาก จนถึงขนาดว่าทำให้หน้าเก่าหลายคนมึนงงไปเลยทีเดียว แต่ถ้าใครเคยเขียน CoffeeScript หรือ Ruby Rails มาแล้ว ก็สามารถสนุกกันต่อได้แบบไม่ขาดตอนกันเลย

  - **Feature** ความสามารถล้นเหลือจริงๆ ทำให้การพัฒนา application ขนาดใหญ่ง่ายขึ้นกว่าเดิมเยอะ แม้ว่าในทางเทคนิกแล้ว ความสามารถต่างๆ จะยังคงถูก port ออกมาเป็น JavaScript แบบเดิมอยู่ก็ตาม เนื่องด้วย Web Browser ยังไม่สนับสนุนเต็มที่ ([ดู babeljs][6])

ส่วนตัวผมคิดว่าสิ่งที่ผลักดันให้ ECMAScript เปลี่ยนแปลงครั้งใหญ่นี้ น่าจะเกิดจากสาเหตุหลักสองสามอย่าง ***—ความเห็นส่วนตัว***

  - **Technology Trends** การเติบโตของอินเตอร์เน็ต ทำให้ JavaScript เป็นภาษาพื้นฐานที่นักพัฒนาทุกคนต้องรู้ โดยเฉพาะอย่างยิ่งเมื่อเกิด node.js ขึ้นมา JavaScript ก็ไม่ได้จำกัดอยู่แค่การพัฒนาบน ​Web Browser อีกต่อไป การเขียนโปรแกรมด้วย JavaScript จึงค่อนข้างหลากหลาย โดยเฉพาะเทคนิกการเขียนโปรแกรมแบบ [Asynchronous Programming][7] ที่ตอบสนองการเชื่อมต่อ API ข้าม Server กันแบบไม่จำกัด

  - **Team Developers** ES6 ถูกออกแบบให้นักพัฒนาทำงานกันเป็นทีมได้สะดวกขึ้น สามารถจัดการ Package การ Reuse โดยไม่ต้องพึ่งพอ Library ข้างนอกอีกต่อไป

  - **Popularity War** สงครามแย่งชิงความนิยมของภาษาโปรแกรมมิ่งเป็นไปอย่างดุเดือด บริษัทยักษ์ใหญ่ทั้งหลายต่างพากันพยายามสร้างภาษาโปรแกรมมิ่งของตัวเองมาประชันกันจนนักพัฒนาแทบอ๊วกแตกกันเลยทีเดียว แต่ภาษาที่เป็นที่ฮือฮากันมากที่สุดคือ Ruby Rails ที่มาพร้อมกับคอนเส็บ Don't repeat yourself (DRY) ทำให้เป็นที่ชื่นชอบของนักพัฒนาทั่วโลก ด้วยการเขียนที่กระชับ syntax ไม่ยืดยาวเยิ่นเย้ออีกต่อไป แม้ว่า JavaScript จะครองความเป็น [Popular Language][8] มายาวนาน (Client side) แต่ถ้าไม่ขยับอะไร มีสิทธิ์ถูก Ruby เบียดตกขอบแน่ๆ (ใครจะรู้ว่า ruby จะไม่ขยับมาเล่นกับ client side ก็ในเมื่อ ​CoffeeScript ยังดื่มเพลินขนาดนั้น)

ด้วยเพราะความที่ ECMAScript6 มีอะไรใหม่เยอะมากพอสมควร ในหนังสือเล่มนี้ ผมจะสรุปเอาเฉพาะที่เราได้ใช้กันบ่อยๆ และเพื่อที่จะได้เห็นภาพมากขึ้น ถ้าเป็นไปได้ ผมจะเทียบกับ ECMAScript5 ไปด้วย

หลายส่วนของ ECMAScript6/7 ยังอยู่ในขั้นตอนการสำเสนอไอเดีย หรือ `Proposal` ซึ่งต้องติดตามความคืบหน้ากันเรื่อยๆ โดยปกติคุณสมบัติที่ `release` แล้ว เราสามารถหาดูได้ใน 

   - [https://developer.mozilla.org/en-US/docs/Web/JavaScript][9]
   -  [https://leanpub.com/understandinges6/read - หนังสือ ES6 แบบเต็มๆ][10]
   -  [http://exploringjs.com/es6/ - เว็บไซต์ให้ความรู้ ES6][11]
   - [https://babeljs.io/ - โปรเจ็คที่ทำให้เราเขียน ES6/7 โดยไม่ต้องรอ Native](https://babeljs.io/)

## The Brief JavaScript Timeline

  - **1995** JavaScript is born as LiveScript
  - **1997** ECMAScript standard is established
  - **1999** ES3 comes out and IE5 is all the rage
  - **2000–2005** XMLHttpRequest, a.k.a. AJAX, gains popularity in app such as   - Outlook Web Access (2000) and Oddpost (2002), Gmail (2004) and Google Maps (2005).
  - **2009** ES5 comes out (this is what most of us use now) with forEach, Object.keys, Object.create (specially for Douglas Crockford), and standard JSON
  - **2015** ES6/ECMAScript2015 comes out; it has mostly syntactic sugar, because people weren’t able to agree on anything more ground breaking (ES7?)

## Javascript Characteristic

ใครที่เริ่มเขียน JavaScript ใหม่ๆ อาจจะแปลกใจกับเรื่องที่ basic ที่สุดเรื่องหนึ่งของ JavaScript นั่นก็​คือ ตัวแปรใน JavaScript มันทำงานแปลกๆ ที่ว่าแปลกคือขอบเขตการทำงานของมัน (Scope context) ซึ่งในภาษาที่มีพื้นมาจากภาษาซี หรือ C-based โดยทั่วไป ตัวแปรมักจะมีขอบเขตของมันแค่ภายในวงเว็บปีกกา `{ ... }` **ณ จุดที่เราประกาศมัน** เช่น

~~~php
<?php

error_reporting(-1);

if (false) {
    $foo = 2;
} else {
    var_dump($foo);
}

/* output
<br />
<b>Notice</b>:  Undefined variable: foo in <b>[...][...]</b> on line <b>8</b><br />
NULL
*/
~~~

ในทำนองเดียวกันของ JavaScript กลับไม่มี error ใดๆ

~~~javascript
// JavaScript

if (false) {
    var foo = 'bar';
    console.log(foo); // bar
} else {
    console.log(foo); // undefined
}
~~~

ผมอดไม่ได้ที่จะเขียนอธิบายเรื่องนี้ไว้ซะหน่อย เพราะถ้าเราไม่เข้าใจ *"ลักษณะพิเศษ หรือ Characteristic"* ของ JavaScript แล้วอาจทำให้การโปรแกรมด้วย ​JavaScript ไม่ราบรื่นนัก

### Variable Hoisting
ลักษณะพิเศษอย่างหนึ่งที่ควรเข้าใจก่อน เมื่อเริ่มเขียน JavaScript นั่นคือการ `Hoisting` ของตัวแปร (ขอไม่แปลเป็นไทยนะครับ ยากสสส์) คุณสมบัตินี้เองที่อธิบายว่าทำไมจากตัวอย่างที่แล้ว ตัวแปร `foo` ถึงไม่มี error ในเมื่อถูกเรียกใช้ใน  block ที่มันไม่ได้ถูกประกาศไว้ ลองดูจากตัวอย่างนี้นะครับ

~~~javascript
// Global scope hoisting

if (false) {
    foo = 'bar';
    console.log(foo); // bar
} else {
    console.log(foo); // undefined
}

console.log(foo); // undefined
~~~

เบื้องหลังแล้ว JavaScript ทำแบบนี้ครับ

~~~javascript
var foo;

if (false) {
    foo = 'bar';
    console.log(foo); // bar
} else {
    console.log(foo); // undefined
}

console.log(foo); // undefined
~~~

เพราะฉะนั้น **Hoisting** ก็คือการทำให้ตัวแปรถูกเรียกใช้ตรงไหนก็ได้ หรือประกาศตรงไหนก็ได้ ภายใต้บริบทเดียวกัน (Scope context) แปลว่าเราจะเรียกใช้มันก่อนหรือหลังการประกาศมันก็ได้ เราจะไม่เจอ Runtime Error ใดๆ

~~~javascript
// Local scope hoisting

function foo() {
    console.log(bar); // undefined

    var bar = 1;

    console.log(bar); // 1
}
~~~

และนี่คือสิ่งที่อยู่เบื้องหลัง

~~~javascript
function foo() {
    var bar;
    console.log(bar); // undefined
    bar = 1;
    console.log(bar); // 1
}
~~~

> `undefined` คือค่าของตัวแปรที่ประกาศขึ้นแล้ว แต่ยังไม่ถูกกำหนดค่าใดๆ
> หากเราพยายามจะเข้าถึงตัวแปรที่ยังไม่ถูกประกาศขึ้น สิ่งที่จะได้คือ `ReferenceError` Runtime Error ไม่ใช่ `undefined`

### Scope & Context
ต่อจากเรื่องลี้ลับ Hoisting สิ่งที่เราควรทำความเข้าใจเป็นลำดับถัดมาของ JavaScript ก็คือเรื่อง `Scope & Context`

  - **Context** คือคำนิยามขอบเขตของตัวแปร `this`  เมื่อพูดถึงอาณาบริเวณของ `this` เราจะพูดว่า `context` ซึ่งหมายถึง ขอบเขตของ `object` ใดๆ เพราะ `this` ใช้อ้างอิงถึง object

  - **Scope** คือคำนิยามขอบเขตของตัวแปรที่เราสร้างขึ้นด้วย `var`  อาณาเขตที่เราจะสามารถเข้าถึงตัวแปรที่เราประกาศด้วย `var` นี้ได้ คือความหมายของคำว่า Scope

ในภาษา JavaScript แบ่ง Scope ออกเป็นสองส่วนหลักๆ คือ **Global scope** และ **Local scope**

- **Global Scope** ใน Browser ตัวแปร `window` ถือเป็น `root` หรือ `global`  scope ของ JavaScript เมื่อใดก็ตามที่เราประกาศตัวแปรขึ้นมา (โดยไม่ได้อยู่ในฟังก์ชั่นใดๆ) ตัวแปรนั้นจะอยู่ใน global scope โดยอัตโนมัติ

~~~javascript
var foo = 'bar';

console.log(foo === window.foo); // true

if (false) {
    var bar = 'baz';
}

console.log(bar === window.bar); // true
~~~

  - **Local Scope** คือตัวแปรที่ประกาศภายในฟังก์ชั่น

~~~javascript
// global scope
var foo = 'bar';

var bar = function() {
    // local scope
    var baz = 'bazz';
}

console.log(baz); // Uncaught ReferenceError: baz is not defined
~~~

### Scope Binding
Scope ใน JavaScript จะเกิดใหม่เมื่อมีการประกาศฟังก์ชั่นใหม่ขึ้นมา

~~~javascript
// scope A
function () {
    // scope B
    function () {
        // scope C
    }
}

function () {
    // scope D
}
~~~

ดูผิวเผินเหมือนกับว่า scope จะอยู่ถายในวงเว็บปีกกา `{ scope context }` แต่ไม่ใช่อย่างนั้น เนื่องจาก scope ไม่ได้เกิดใหม่ในคำสั่งเหล่านี้ แต่ถูก `hoisting` แทน

  - `for (var i = 0; i < 10; i++) { console.log(i) }`
  - `if () { .. }`
  - `switch () { .. }`
  - `while { .. }`


### Lexical & Scope Chain
คล้ายๆ [Scope inheritance ใน AngularJs](https://github.com/angular/angular.js/wiki/Understanding-Scopes#angular-scope-inheritance) Scope ที่เกิดขึ้นเมื่อสร้างฟังก์ชั่นขึ้นมาใหม่ สามารถเข้าถึง scope ของฟังก์ชั่นอื่นที่ครอบมันอยู่ได้ กรณีสร้างฟังก์ชั่นซ้อนๆ กัน พูดอีกอย่างคือ JavaScript จะมองหาตัวแปรใน local scope ก่อน ถ้าไม่เจอจะไล่ขึ้นไปเรื่อยๆ จนถึง global scope

~~~javascript
function one() {
    var foo = 1;
    two();
    function two() {
        foo = 2;
        three();
        function three() {
            foo = 3
            four();
            function four() {
                console.log(foo);
            }
        }
    }   
}

one(); // 3
~~~

จากตัวอย่าง function ที่ถูกเรียกหลังสุดคือ `four()` ซึ่งพิมพ์ค่าของตัวแปร `foo` ที่อยู่นอก function ของตัวเอง แต่ก็ยังได้ค่า `3` เพราะ `four()` อยู่ภายใน `chain` ของ `three()` นั่นเอง

~~~javascript
// หรือ
var foo = 0;
function one() {
    foo = 1;
    two();
    function two() {
        foo = 2;
        three();
        function three() {
            foo = 3
            four();
            function four() {
                console.log(foo);
            }
        }
    }   
}

one(); // 3
~~~

ตัวอย่างข้างบนเป็นการทำงานของ `scope chain` ไล่ไปจนถึง `global scope`

~~~javascript
function one() {
    console.log(foo);
    two();
    function two() {
        var foo = 1;
    }   
}

one(); // Uncaught ReferenceError: foo is not defined
~~~

ตัวอย่างนี้ Scope Chain ไม่สามารถทำงานแบบย้อนกลับได้ (Backward)

### Closure Scope
Closure คือค่าของตัวแปรที่เป็นฟังก์ชั่น หรือค่า return ของฟังก์ชั่นที่เป็นฟังก์ชั่น

~~~javascript
function foo() {
    var bar = 1;
    return function() {
        return bar;
    }
}

var closure = foo();
closure(); // 1
~~~

ส่วน Scope ใน Closure น่าสนใจมากนะครับ ลองพิจารณาตัวอย่างอีกอัน

~~~javascript
function foo() {
    var bar = 1;
    return function() {
        return bar;
    }
}

var closure = foo();

function baz() {
    var bar = 3;
    return closure();
}

baz(); // 1
~~~

จากตัวอย่าง ตัวแปร `closure` ถูกเรียกใช้ใน scope ของ `baz` *(baz execution context)* แต่ก็ยังคงให้ค่าเป็น `1` เหมือนเดิม แม้ว่า `baz` จะประกาศตัวแปร `bar` ขึ้นมาใน scope ตัวเองก็ตาม เป็นดังนี้เพราะ ***closure มี scope ของตัวเองจากตอนที่มันถูกสร้างขึ้น*** ในที่นี้มันถูกสร้างภายใต้ scope ของ `foo` ซึ่งก็ย้อนไปเข้าลักษณะของ scope chain ก่อนหน้านี้

และด้วยความสามารถนี้เอง เราจึงสามารถประยุกต์ใช้หลักการ `public`, `private` scope ในความหมายของ  OOP ได้ (ซึ่งจะอธิบายภายหลัง)

~~~javascript
var aClass = (function() {
    var privateProperty = 'foo';
    
    var privateMthod = function bar() {
        return privateProperty;
    }
    
    return {
        publicProperty: 'bazz',
        
        publicMethod: function() {
            return privateProperty;
        }
    };
})();
~~~

มีบางสิ่งที่อาจทำให้เราสับสนเกี่ยวกับ closure scope แรกๆ ตัวผมเองก็มึนงงกับ closure scope เหมือนกัน ลองดูตัวอย่างนี้นะครับ

~~~javascript
var foos = [];
for (var i = 0; i < 10; i++) {
    foos[i] = {
        closure: function() {
            return i;
        }
    };
}

for(var n in foos) {
    console.log(foos[n].closure());
}

// Output: 10 (10 times)
~~~
จากตัวอย่างข้างบน ดูผิวเผินเราคาดหวังว่าจะให้ได้ค่าที่ return ออกจาก closure เป็น `0-9` แต่กลับได้ `10` ซ้ำกัน 10 รอบ ทั้งนี้ก็เนื่องจากกว่า `var i` ใน `for` เป็น global scope ของ `closure` ณ ตอนที่มันถูกสร้างขึ้น ค่าที่ได้จาก `i` จึงเป็นค่าล่าสุดที่ `i` ถูก assign ค่าให้ ในที่นี้เมื่อสิ้นสุด `for` แล้ว i มีค่าเป็น `10` และเราเรียกใช้งาน (execute) `closure` ภายหลังจากนั้น ค่าที่ได้จึงเป็น `10` เสมอ

> `var i` ใน `for` มีค่าเท่ากับ `var i; for(i = 0; ..) { ... }` จากคุณลักษณะของ variable hoisting

เพราะฉะนั้นแล้ว ถ้าอยากได้ค่าที่เราคาดหวัง (0-9) จึงต้องปรับโปรแกรมดังนี้

~~~javascript
var foos = [];
for (var i = 0; i < 10; i++) {
    foos[i] = {
        closure: function(i) { return function() {
            return i;
        }}(i)
    };
}

for(var n in foos) {
    console.log(foos[n].closure());
}

// Output:
// 0
// 1
// 2
// 3
// 4
// 5
// 6
// 7
// 8
// 9
~~~

ก็คือกำหนด chain parent scope ใหม่ให้ closure ของเรานั่นเอง — ลองปรับให้ลดความสับสนลงอีกซักนิด

~~~javascript
var foos = [];
for (var i = 0; i < 10; i++) {
    foos[i] = {
        closure: function(n) { return function() {
            return n;
        }}(i)
    };
}
~~~

> function(n) { ... }(i); คือการเรียกใช้งาน (execution) ฟังก์ชั่นทันที่พร้อมกับการประกาศ `i` ก็คือ `argument` ที่ส่งเข้าไปเป็น `n` `parameter` นั่นเอง — [IIFE][6]


เป็นไงกันบ้างครับ รู้สึกดีขึ้น หรือว่าตึ๊บๆ กับ Scope ของ JavaScript กันยังไงบ้างครับ ผมอยากจะบอกว่า ทั้งหมดทั้งปวงนี้เป็นทั้งเสน่ห์และความน่าสับสนในการใช้งานตัวแปรใน JavaScript ES5 ซึ่งพระเอกของเราในที่นี้ก็คือ `var` หรือคำประกาศตัวแปรของเรานั่นเอง


## Introducing to `const` and `let`

ถึงตรงนี้ก็เหมาะสมที่ผมจะแนะนำนักแสดงนำหน้าใหม่ในภาค ES6 เข้ามาสร้างสีสรรประชันกับ `var` กันได้แล้วนะครับ เขาผู้นั้นก็คือ `let` กับ `const` ผู้ซื่อสัตย์นั่นเอง

ใน ES6 เรายังสามารถใช้ `var` ได้เหมือนเดิม เพียงแต่จากความน่าฉะงนสนเท่ห์ของมัน ซึ่งอาจทำให้เรามึนงง อันที่จริงก็คือซึ่งอาจนำเราไปสู่ `Bug` ที่ไม่คาดหวัง ES6 ได้นำเสนอการสร้างตัวแปรใหม่ เพิ่มขึ้นอีก 2 แบบ คือ

  - **let** ใช้สำหรับสร้างตัวแปรที่สามารถเปลี่ยนค่ามันได้
  - **const** ใช้สำหรับสร้างตัวแปรที่ไม่สามารถเปลี่ยนค่าได้อีก *(constanst หรือ ค่าคงที่นั่นเอง)*

การใช้งานก็ง่ายดายเหมือน `var`

~~~javascript
var foo = 1;
let bar = 2;
const bazz = 3;
~~~

### การใช้งาน `const`
ข้อควรจำง่ายๆ สำหรับการใช้งาน `const`

 - ไม่สามารถกำหนดค่าให้มันใหม่ได้
 - ไม่สามารถประกาศซ้ำกับตัวแปรที่ประกาศแล้วอีกได้
 - ต้องมีค่าเริ่มต้นเสมอ

~~~javascript
const bazz = 3;

bazz = 4; // will throw error

const bazz;  // missing initialization, will throw error

var foo = 1;
let bar = 2;

// throw an error
const foo = 1;
const bar = 2;

// object declaration
const car = {
    name: 'Ford'
};

// works
car.name = 'Toyota';

// throws an error
car = {
    name: 'Honda'
};
~~~

### การใช้งาน `let`
`let` ใกล้เคียงกับ `var` ต่างการตรงที่การ `hoisting` และ `scope` ของมัน อันที่จริงก็คือ `let` กลับไปสู่สไตล์ของภาษาจำพวก C-based ซึ่งมี scope ของตัวแปรอยู่ภายใต้ วงเว็บปีกกา `{ ... }` และ ภายในฟังก์ชั่นของใครของมัน หรือที่เรียกว่า `Block-Level Declarations`

~~~javascript
if (true) {
    let foo = 1;
    console.log(foo) // 1
} else {
    console.log(foo) // throw error
}

console.log(foo) // throw error
~~~

 - ไม่สามารถประกาศตัวแปรด้วย `let` ซ้ำกับ `var` ได้ภายใน scope เดียวกัน

~~~javascript
var foo = 1;
let foo = 2; // syntax error

if (true) {
    let foo = 2; // OK, Does not throw an error
}
~~~

 - อย่าลืมว่า `let` ไม่มีคุณลักษณะ `hoisting` แล้ว scope ของมันอยู่ใน `{
   ... }`

~~~javascript
// The Temporal Dead Zone
if (true) {
    console.log(typeof bar);  // ReferenceError!
    let bar = 2;
}

// var style
for (var i = 0; i < 10; i++) {
    console.log(i);
}

// i is still accessible here
console.log(i);

// let style
for (let i = 0; i < 10; i++) {
    console.log(i);
}

// throws an error
console.log(i);
~~~

 - ความสับสนเรื่อง `var hoisting` ใน `for loop`

~~~javascript
// var style
var foos = [];
for (var i = 0; i < 10; i++) {
    foos[i] = {
        closure: function(n) { return function() {
            return n;
        }}(i)
    };
}

// let style
let foos = [];
for (let i = 0; i < 10; i++) {
    foos[i] = {
        closure: function() {
            return i; // :) let เกิดใหม่ทุกครั้ง
        }
    };
}
~~~

> คุณสมบัตินี้ใช้ได้ใน `for-in` และ `for-of` ด้วย

> อันที่จริง `let` เกิดใหม่ทุกครั้งใร `for` เป็นการกำหนดคุณสมบัติโดยเฉพาะ (Specification) ของ ES6 ซึ่งไม่ใช่คุณสมบัติเรื่อง `Non-hoisting` แต่อย่างใด (ว่ายังงั้น)

### Globals scope ใน `let` และ `const` กับ `var`

~~~javascript
// var style
var foo = 1;
console.log(foo === window.foo); // true


// let / const style
let foo = 1;
console.log(foo === window.foo); // false

const bar = 2;
console.log(bar === window.bar); // false
~~~

### สรุปการใช้งาน `var` `let` `const`
  - `let` และ `const` เป็นการสร้างตัวแปรที่มี scope อยู่แค่ block `{ ... }` ที่มันถูกสร้างขึ้นเท่านั้น 
  - `let` และ `const` ไม่มีคุณสมบัติ `hoisting` เหมือน  `var`
  - มีข้อควรระวัง `let` และ `const` คือ การใช้คำสั่ง `typeof`   เช็คตัวแปรก่อนที่มันจะถูกประกาศขึ้น เราจะได้รับ `ReferenceError` แทนที่จะเป็น `undefined` เหมือนใน `var` (The Temporal Dead Zone — TDZ)
  - `let` และ `const` ทำงานคล้าย `var` ยกเว้นใน `for loop` ซึ่ง `let` จะเกิดใหม่ทุกครั้งในแต่ละการวน `loop`
  - `const` ใช้ใน `for loop` ไม่ได้ (เว้นเสียแต่ว่าคุณจะมี loop รอบเดียว ซึ่งคงไม่ใช่จุดประสงค์ของ `for`)
  - ควรใช้งาน `const` เป็นพื้นฐาน
  - ใช้ `let` สำหรับตัวแปรที่จะมีการเปลี่ยนค่าใหม่
  - ~~หลีกเลี่ยงการใช้ `var`~~ ใช้ `var` เฉพาะกรณีที่คุณรู้แน่แก่ใจว่ากำลังทำอะไรอยู่ :)


## การหายไปของเซมิโคลอน (;)

ES6 ไม่ต้องปิดประโยคคำสั่งด้วย `;` อีกต่อไปแล้ว งานนี้สาวก `Ruby` ร้อง `YMCA ...` เอ้ย `DRY!`

~~~javascript
// ES5
var foo = 'foo';
var bar = function() { return 'bar'; };

// ES6
var foo = 'foo'
var bar = () => 'bar' // "O"
~~~


## Arrow Functions
Arrow Functions หรือ "fat arrow" นับเป็นการเปลี่ยนแปลงที่ว้าวมากอย่างหนึ่งใน ES6 แต่ก็อาจเป็นที่มึนหัวมากที่สุดอย่างหนึ่งสำหรับคนที่ชินกับ ES5 อยู่แล้ว (ไม่ใช่กับเหล่าสาวก CoffeeScript แน่ๆ)

**ใน ES5 เรา สามารถประกาศ function ได้ 2 แบบหลักๆ คือ**

*1. Function Expression*

~~~javascript
var foo = function (bar) { return bar; }
~~~

*2. Function Definition*

~~~javascript
function foo(bar) { return bar; }
~~~

**ใน ES6 Arrow Functions ทำให้การประกาศ function สนุกขึ้น**

~~~javascript
var foo = bar => bar
~~~
อ่า! แปลกตาดีนะครับ มันคือะไร?

~~~javascript
var ชื่อฟังก์ชั่น = พารามิเตอร์ => รีเทิร์นค่า
~~~

อืมมม! เข้าท่าแฮะ


**แรกๆ นักพัฒนาหน้าเก่าอาจต้องทดหลายสิ่งไว้ในใจนะครับ**

*1. ถ้าฟังก์ชั่นมี parameter เดียว ไม่ต้องใช้วงเล็บครอบ parameter ก็ได้*

~~~javascript
var foo = (bar) => bar
// หรือ
var foo = bar => bar
~~~

> Parameters vs Arguments
> 
> - **Parameters** คือ ตัวแปรที่ใช้รับค่าเข้าไปใน function — `function foo(parameter) {}`
> - **Arguments** คือ ค่าที่ถูกส่งเข้าไปใน function ตอนที่มันถูกเรียกใช้ — `foo(argument)`
> 

*2. ถ้าฟังก์ชั่นไม่มี parameter เลย ก็ยังต้องใช้ `()`*

~~~javascript
var foo = () => 'hi, bar'
~~~

*3. ไม่ต้องใช้คำสั่ง return ก็ได้ ถ้าเขียน body ของฟังก์ชั่นในบรรทัดแรกต่อจาก arrow function (`=>`) ทันที*

~~~javascript
var foo = (bar) => return bar
// หรือ
var foo = bar => bar
~~~

*4. ไม่ต้องใช้วงเว็บปีกกาครอบ body ของฟังก์ชั่นก็ได้*

~~~javascript
var foo = (bar) => { bar }
// หรือ
var foo = bar => bar

// แต่หากต้องการ return Empty Object ไม่สามารถใช้แบบนี้ได้
var foo = () => {}
// ต้องใช้แบบนี้
var foo = () => ({})
~~~

*5. Context `this` ของ arrow function คือ parent context ของมัน ตอนที่มันถูกสร้าง*

สิ่งที่ว้าวจริงๆ ของ arrow functions คือเมื่อมันใช้เป็น callback function

~~~javascript
// ES5
fetch('/api').then(function(res) {
    return res.toJson();
});

// ES6
fetch('/api').then(res => res.toJson())
~~~

ที่ว่าว้าวคือ arrow functions จัดการกับ `this` scope ของ callback function ด้วย

*— ES5 Scope Binding*

~~~javascript
$('.btn').click(function(e) {
    var me = this;
 
    me.disabled = true;
    fetch('/api').then(function(res) {
        me.disabled = false;
        return res.toJson();
    });
});

// หรือ — ใช้ bind
$('.btn').click(function(e) {
    this.disabled = true;

    fetch('/api').then(function(res) {
        this.disabled = false;

        return res.toJson();
    }.bind(this));
});
~~~

*— ES6 Scope Binding (มันว้าวจริงๆ)*

~~~javascript
$('.btn').click(e => {
    this.disabled = true

    fetch('/api').then(res => {
        this.disabled = true

        return res.toJson()
    })
})
~~~

แต่เดี๋ยวก่อน! ถ้า `Arrow Function` จัดการกับ `this` scope โดยให้เป็น `this` ในบริบทของ `parent` แบบนี้ แปลว่า Arrow function ไม่ได้สร้าง `this` scope ของตัวเองขึ้นมาเหมือน function ปกติ นั่นหมายถึงคุณไม่สามารถใช้คำสั่ง `new` เพื่อสร้าง `instance` ของมันได้ เพราะว่ามันไม่มี `prototype` เป็นของตัวเองนั่นเอง

เอาเป็นว่าจำไว้ว่า `this` scope ของ arrow function ก็คือ `parent` ของมัน ณ ขณะที่ประกาศมันนั่นเอง

## Default Parameters
ES6 มีค่าเริ่มต้นให้ฟังก์ชั่นพารามิเตอร์เหมือนชาวบ้าน (ภาษาอื่น) แล้ว :)

~~~javascript
// ES5
var animal = function(name, age, sound)
{
    var age = age || 1;
    var sound = sound || 'Foww';
 
    // ...
}

// ES6
var animal = function(name, age = 1, sound = 'Foww')
{
    // ...
}

animal('Tiger')

var animal = function({ age: 1, sound: 'Foww'} = {})
{
    console.log(age) // ...
}

animal({ name: 'Tiger', age: 2 })
~~~

## Template Literals
ES6 มีความสามารถในการต่อสตริงด้วยระบบ template โดยการใช้ syntax `${ชื่อตัวแปร}`

~~~javascript
// ES5
var animal = 'Cat';
var cat = 'This is a: ' + animal + '.';

// ES6
var animal = 'Cat'
var cat = `This is a: ${animal}.`
~~~

> String template ใน ES6 ใช้เครื่องหมาย \`...\` แทนเครื่องหมาย quote หรือ single quote `'...', "..."`


## Multi-line Strings
การต่อสตริงหลายบรรทัดใน ES6 ทำได้ง่ายมากขึ้น

~~~javascript
// ES5
var text1 = 'React makes it painless to create interactive UIs.\r\n'
    + 'Design simple views for each state in your application, \r\n'
    + 'and React will efficiently update and render just the right \r\n'
    + 'components when your data changes.';

var text2 = 'Declarative views make your code more predictable \
    and easier to debug.';

// ES6
var text1 = `React makes it painless to create interactive UIs.
    Design simple views for each state in your application,
    and React will efficiently update and render just the right
    components when your data changes.`

var text2 = `Declarative views make your code more predictable
    and easier to debug.`
~~~

สะดวกขึ้นเยอะ! และอย่าลืมนะครับว่าเรายังสามารถใช้ `${variable}` เพื่อใส่ค่าตัวแปรเข้าไปได้

## Destructuring Assignment
เป็นคำสั่งในการกำหนดตัวแปรจาก key ของ object หรือ ค่าของ array คล้ายๆ กับ[ฟังก์ชั่น list ของ php][4]

~~~javascript
// Example data
var Customer = {
    firstName: 'John',
    lastName: 'Doe',
    info: {
	    phoneNumber: 1234
    }
}

// Destructuring
var { firstName, lastName, info: { phoneNumber } } = Customer
console.log(firstName) // John
console.log(lastName) // Doe
console.log(phoneNumber) // 1234
~~~

พูดง่ายๆ คือ อะไรก็ตามที่ return ค่าเป็น object เราสามารถทำความสามารถ Destructuring ในการสร้างตัวแปรได้เลย เช่น

~~~javascript
// ES5
var gutil = require('gulp-util')

console.log(gutil.env); // ...

// ES6
var { env } = require('gulp-util')
~~~

แถมยังทำงานกับ Array ได้อีกด้วย

~~~javascript
// Example array data
var list = [1, 2, 3, 4];

// Array Destructuring
var [ one, two, three, four ] = list
~~~

ความสามารถนี้เป็นที่นิยมและใช้กันจนเป็นพื้นฐานใน ES6 เนื่องจากทำให้การเขียนตัวแปรสั้นลงมาก

## Enhanced Object Literals
อะไรคือ Object Literals? ก็ JSON object นั่นแหละครับ เพียงแต่ว่า ถ้าประกาศใน JavaScript เราสามารถใส่ฟังก์ชั่นเข้าไปได้ด้วย

~~~javascript
// Example array data
var customer = {
    firstName: 'John',
    lastName: 'Doe',
    getFullName: function () {
        return this.firstName + ' ' + this.lastName;
    }
};
~~~

สำหรับความสามารถที่เรียก Enhanced Object Literals ก็คือ

### 1. Property value shorthand

~~~javascript
// ES6
function getOptions(options, data)
{
    return { options, data };
}

// มีค่าเท่ากับ ES5
function getOptions(options, data)
{
    return {
        options: options,
        data: data
    };
}
~~~
พูดง่ายๆ คือ ถ้าชื่อ `property` ตรงกับชื่อตัวแปรที่เป็น `value` ก็ไม่ต้องเขียนชื่อ property ก็ได้

### 2. Method definition shorthand

~~~javascript
// Example array data
var customer = {
    firstName: 'John',
    lastName: 'Doe',
 
    getFullName {
        return `${this.firstName}  ${this.lastName}`
    }
};
~~~

ไม่ต้องเขียน keyword `function`, `key`, `:` สำหรับประกาศฟังก์ชั่นใน  Literal object

> อืมมม, โดยส่วนตัวผมไม่ชอบ feature เหล่านี้เท่าไร มันดูมักง่ายไปนิด ;) แต่ใช้ไปใช้มาก็ชินครับ

### 3. Computed property keys
การประมวลผล expression ในชื่อ property key

~~~javascript
// ES6
function getOptions(prefix, data)
{
    return {
        // property
        [prefix + 'key']: data,

        // function
        ['get' + prefix]() => data,
    };
}

// มีค่าเท่ากับ ES5
function getOptions(prefix, data)
{
    var result = {};
    result[prefix + 'value'] = data;
 
    result['get' + prefix] = function () {
        return data;
    };
 
    return result;
}
~~~

> อันนี้แจ่มมาก

## Property Accessor (Setter/Getter)
หลักการทั่วไปอย่างหนึ่งของ OO คือการ encapculation data ซึ่งหมายถึง `property` ใน object ควรได้รับการปกป้อง

ความหมายโดยผิวเผินของ encapculation คือ property ควรเป็น `private` หรือ `protected` เพื่อไม่ให้ถูกเปลี่ยนแปลงค่าได้ตามอำเภอใจ ... นั่นก็ฟังดูโอเค

แต่ถ้าจะว่ากันให้ถูกต้องความหมายของ encapculation คือ **"Object ควรประกอบด้วย valid state เท่านั้น"** หมายความว่า ค่าใดๆ ของ object ที่จะถูกเปลี่ยนแปลง (Change object state) ควรได้รับการตรวจสอบก่อนเสมอ

และวิธีที่ง่ายที่สุดสำหรับการทำสิ่งนี้คือ ทุกครั้งที่จะทำการเปลี่ยนแปลงค่าของ object ควรทำผ่าน method แทนที่จะกำหนดค่าไปที่ property โดยตรง ทั้งนี้เพราะเราสามารถเขียน code ตรวจสอบความถูกต้องของค่าที่ถูกส่งเข้ามาได้ ไม่ว่า property นั้นๆ จะเป็น `public, private หรือ protected` ก็ตาม

~~~javascript
class Personal
{
    constructor (name, age)
    {
        this.name = name;
        this.age = age;
    }

    // getter
    get age () => this.age
 
    // setter
    set age (age) =>
        if (isNaN(age) {
            throw new Error('Age must to be numberic.')
        }
     
        this.age = age
}

let person = new Personal('John Doe', 70)

// This's will throw error "Age must to be numberic."
person.age = "He was deaded!"
~~~

เท่านี้ property ใน Object ของเราก็จะถูกปกป้องราวกับไข่ในท้องไก่แล้ว ต้องยกความดีความชอบให้ `property accessor` เขาล่ะ



## Spread syntax
การกระจาย arguments, สมาชิกใน array, หรือ การสร้างตัวแปรแบบยกชุดด้วยวิธี `Destructuring assignment` วิธีการนี้เป็นที่นิยมอย่างมากในภาษาโปรแกรมมิ่งสมัยใหม่ (เข้าใจว่ามาจาก Ruby) แม้แต่ใน React เองก็นิยมมากตอนเรากำหนดค่า Properties ให้กับ Component

~~~javascript
function Component()
{
    let properties = { foo: 1, bar: 2 }
    
    return <Component ...properties />
}

// <Component foo="1" bar="2" />
~~~

ลองดูตัวอย่าง [Spread syntax กันเต็มๆ ที่นี่][7] หรืออันที่เป็น [proposal][8] นะครับ

## Native Promise
ES6 สนับสนุน Promise แล้ว ใครที่ยังใหม่มากๆ สำหรับแนวคิดของ `Promise` เผื่อจะเป็นการช่วยจำกัดประเด็นในการค้นคว้าลงได้บ้าง ผมก็อยากสรุปแนวคิดของ `Promise` สั้นๆ 

Promise คือการการันตี response จาก Asyncronize โดย response ที่คืนกลับมาจะมีแค่ 2 อย่างคือ
  - `fullfill: สำเร็จ`
  - `failed: ไม่สำเร็จ`

รูปแบบการใช้งาน Promise เป็นความพยายามที่จะลดความซับซ้อนของ Asyncronize โปรแกรมมิ่งลง โดยให้รูปแบบการเขียนใกล้เคียงกับ Synchronize โปรแกรมมิ่ง

เพื่อไม่ให้หนังสือเล่มนี้กลายเป็น JavaScript Book [ใครสนใจเรื่อง Promise อ่านได้ที่นี่][9]


## Class Syntax
แรกเริ่มเดิมทีเราใช้ JavaScript เพียงแค่เป็น Script เพื่อจัดการกับ Html ให้สามารถ Interactive ได้ แต่เมื่อมันเริ่มใช้เป็นภาษาสำหรับพัฒนา application ใหญ่ขึ้นเรื่อยๆ ความสามารถแบบภาษา script จึงค่อนข้างเป็นข้อจำกัดสำหรับนักพัฒนา แน่นอนว่าการพัฒนาที่ใหญ่ขึ้น ภาษาโปรแกรมมิ่งอย่าง Java, C++ หรือ C# ที่สนับสนุนการเขียนแบบ Object-Oriented (OO) อย่างเต็มที่ ย่อมทำให้การพัฒนามีความสะดวก รวดเร็ว และรัดกุมมากขึ้น แม้ว่าเราจะเขียน JavaScript แบบ OO ได้ แต่มันก็ถือว่ามีความสามารถน้อยมากถ้าเทียบกับภาษา OO โดยตรง

### การสร้าง Class
ES6 มี keyword `class` สำหรับการประกาศคลาสโดยตรง และ function ชื่อ `constructor` สำหรับเป็น constructor ของคลาส

~~~javascript
// ES5
var Animal = (function()
{
    function Animal(name, age)
    {
        this.name = name;
        this.age = age;
    }
    
    return Animal;
}());

// ES6
class Animal {
  constructor(name, age) {
    this.ame = name;
    this.age = age;
  }
}
~~~

การประกาศคลาสด้วย keyword `class` จะไม่มีคุณสมบัติ `Hoisting` เหมือน `function` แปลว่าคุณจะเรียกใช้มันก่อนที่จะประกาศเหมือนที่เคยทำกับฟังก์ชั่นไม่ได้แล้ว

~~~javascript
// ReferenceError
var p = new Animal();

class Animal {}
~~~

เราสามารถประกาศคลาสแบบเป็นตัวแปร หรือ expression ก็ได้

~~~javascript
var Animal = class {
  constructor(name, age) {
    this.name = name
    this.age = age
  }
};
~~~

### Class Methods
สมาชิกของ class ใน ES6 สามารถเขียนได้ง่ายขึ้นมาก `constructor` เป็นฟังก์ชั่นพิเศษสำหรับการเป็น class constructor ฟังก์ชั่นอื่นๆ จะเป็น methods ของคลาส

~~~javascript
// ES5
var Animal = (function()
{
    function Animal(name, age)
    {
        this.name = name;
        this.age = age;
    }

    Animal.prototype.getNameWithAge = function() {
        return 'Name: ' + this.name + ', Age: ' + this.age;
    }

    return Animal;
}());

// ES6
var Animal = class {
  constructor(name, age) {
    this.name = name
    this.age = age
  }

  // getter
  get age() {
    return age || 0
  }

  // public method
  getNameWithAge() {
    return `Name: ${this.name}, Age: ${this.age}`
  }
};
~~~


### Class Visibility
การกำหนด class visibility เช่น `private`, `protected`, `public`, `final` เป็นต้น เป็นความสามารถพื้นฐานใน OOP แต่ใน JavaScript ใช้การประยุกต์เทคนิกต่างๆ สำหรับทำสิ่งเหล่านี้ เช่น **"การตั้งชื่อให้สื่อความหมาย"** หรือ **"การเขียนโค๊ดคอมเม้นกำกับ"**

~~~javascript
// ES5
var Animal = (function()
{
    // private scope
    var _foo = 1;
    
    // private method
    function _bar() {
        console.log(this.name);
    }
    
    function Animal(name, age)
    {
        this.name = name;
        this.age = age;
        
        /**
         * @private
         */
        this._foo = 1;
        
        // bind `_bar` into `this` context
        _bar.bind(this);
    }

    /**
     * @return string
     * 
     * @protected
     */
    Animal.prototype.getNameWithAge = function() {
        return 'Name: ' + this.name + ', Age: ' + this.age;
    }

    return Animal;
}());
~~~

> เทคนิกการทำ private data แบบต่างๆ [http://2ality.com/2016/01/private-data-classes.html][10]

ใน ​ES6 คุณสมบัติเกี่ยวกับ class visibility ยังเป็น `Proposal` หรืออยู่ระหว่างขั้นตอนการนำเสนอแนวคิด ซึ่งต้องติดตามกันเรื่อยๆ 

ส่วนการกำหนด `public` property ใน ES6 ก็สามารถทำผ่าน `constructor` ได้เลย

~~~javascript
// ES6
class Animal {
  constructor(name, age) {
    this.name = name
    this.age = age
  }
}

var cat = new Animal('aCat', 2)
console.log(cat.name) // aCat
~~~

อาจดูไม่สวยงามนักถ้าเรามี property เยอะมากๆ แต่ใน ES7 เราจะสามารถกำหนด public property ไว้นอก constructor ได้ 

~~~javascript
// ES7
class Animal {
  color = 'black'
  
  constructor(name, age) {
    this.name = name
    this.age = age
  }
}

var cat = new Animal('aCat', 2)
console.log(cat.color) // black
~~~

หรือหากใช้ [babeljs][12] ในโปรเจ็ค เราก็จะสามารถใช้งานคุณสมบัติของ ES7 ได้เช่นกัน ซึ่งจะทำให้ code ใน constructor ไม่ดูรกรุงรังอีกต่อไป

### Static Members
ES6 เพิ่ม `static` keyword มาให้เราใช้งานเพื่อสร้าง static method

~~~javascript
// ES5
var Animal = (function()
{
    function Animal(name, age)
    {
        this.name = name;
        this.age = age;
    }

    Animal.SomeStaticMethod = function() {
        return 'foo';
    }

    return Animal;
}());

console.log(Animal.SomeStaticMethod()); // foo

// ES6
var Animal = class {
  constructor(name, age) {
    this.name = name
    this.age = age
  }

  static SomeStaticMethod() {
    return 'foo'
  }
};
~~~

และเช่นเคย ใน ES7 หรือ [babeljs][12] โปรเจ็ค เราสามารถใช้งาน static property ได้ด้วย

~~~javascript
var Animal = class {
  static Foo = 'bar';
  
  constructor(name, age) {
    this.name = name
    this.age = age
  }

  static SomeStaticMethod() {
    return 'foo'
  }
};

// console.log(Animal.Foo) // bar
~~~

> `static` method ใน ES6 ไม่สามารถ return `this` context ได้เหมือนใน ES5


### Inheritance
การสืบทอดคุณสมบัติของ class

~~~javascript
// ES5
var Cat = (function()
{
    function Cat(name, age)
    {
        // call parent constructor
        Animal.call(this, name, age);
    }
 
    Cat.prototype = new Animal();
    Cat.prototype.constructor = Cat;
 
    Cat.prototype.speak = function ()
    {
        return 'meowww'
    }
}());
~~~

การสืบทอด class ใน ES5 ทำได้ด้วยเทคนิกการเรียกใช้ function  `Animal` ในบริบท (context) ของ function Cat เท่านี้ Cat ก็จะสืบทอด properties ของ `Animal` มา และเราก็กำหนดค่า `prototype` ของ `Cat` ให้เป็น `instance` ของ `Object Animal` 

;) ซับซ้อนไปนิด แต่ก็ใช้ได้!!

ส่วนใน ES6 มี keyword `extends` สำหรับการทำ `inheritance` โดยเฉพาะ และมี keyword พิเศษ `super` สำหรับการเข้าถึงคลาสแม่

~~~javascript
class Cat extends Animal
{
    constructor(name, age) {
       super(name, age);
       
       // other logic
    }
 
    speak() {
       // call super class method
       super.speak()
       
       // .. logic
    }
}
~~~

การเขียน class ใน ES6/7 ง่ายและสนุกขึ้นเยอะใช่ไหมครับ!

## Modules
การจัดการ package หรือการ reuse code ของ ES6 ทำได้ง่ายมากโดยไม่ต้องใช้ Library ภายนอกจำพวก `AMD` หรือ library ยอดนิยม เช่น [requirejs][13] อีกต่อไป เพราะ ES6 มี `import`, `export` สำหรับจัดการ modular package

~~~javascript
//  lib/math.js
export function sum (x, y) { return x + y }
export var pi = 3.141593

//  someApp.js
import * as math from "lib/math"
console.log("2π = " + math.sum(math.pi, math.pi))

//  otherApp.js
import { sum, pi } from "lib/math"
console.log("2π = " + sum(pi, pi))
~~~

- export
- export default
- export index.js


[1]:	https://en.wikipedia.org/wiki/ECMAScript
[2]:	https://tc39.github.io/ecma262/
[3]:	https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain
[4]:	https://github.com/angular/angular.js/wiki/Understanding-Scopes
[5]:	https://leanpub.com/understandinges6/read#leanpub-auto-var-declarations-and-hoisting
[6]:	https://babeljs.io
[7]:	https://stackoverflow.com/questions/748175/asynchronous-vs-synchronous-execution-what-does-it-really-mean
[8]:	http://spectrum.ieee.org/static/interactive-the-top-programming-languages-2016
[9]:	https://developer.mozilla.org/en-US/docs/Web/JavaScript
[10]:	https://leanpub.com/understandinges6/read
[11]:	http://exploringjs.com/es6/
[12]: https://babeljs.io
[13]: http://requirejs.org

