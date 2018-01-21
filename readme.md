# Virtual dom

In DOM api javascript trated full html document as object. This html is real dom. So what is virtual dom? Virtual dom is creating html elment in js. We can build full html using virtual dom and mounted to real dom. In this video, we made a navigation virtual dom and at the end mounted that virtual dom in our real dom. Following method we used today.      

* `document.createElement`
* `document.createTextNode`
* `element.appendChild`
* `element.setAttribute`


Lot of modern js framework using virtual dom facility. Like `react js` and  `vue js`.  Js framework which use virtual dom is pretty fast than other js library. So you may find using `react js` and `vue js` we can build website which is very fast     


In following code we create virtual dom for navigation and appended to real dom.   

~~~js
var ul = document.createElement('ul');
var li1 = document.createElement('li');
var a1 = document.createElement('a');
a1.setAttribute('href', '#');
li1.appendChild(a1);
var a1text = document.createTextNode('Home');
a1.appendChild(a1text);
var li2 = document.createElement('li');
var a2 = document.createElement('a');
a2.setAttribute('href', '#');
var a2text = document.createTextNode('About');
a2.appendChild(a2text);
li2.appendChild(a2);
var li3 = document.createElement('li');
var a3 = document.createElement('a');
a3.setAttribute('href', '#');
var a3text = document.createTextNode('Contact');
a3.appendChild(a3text);
li3.appendChild(a3);
ul.appendChild(li1);
ul.appendChild(li2);
ul.appendChild(li3);
document.body.appendChild(ul);
~~~


