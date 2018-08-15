# daily-javascript-q94

You have the following code:

```javascript
<body> 
      <div id="main"> 
           <p>paragraph 1</p> 
           <p class="target">paragraph 2</p> 
           <p>content 2</p> 
           <p class="target">Some more content here</p> 
           <p>paragraph 3</p> 
      </div> 
      <div> 
           <p class="target"> 
                <span>paragraph 4</span> 
                <div class="target">content 4</div> 
           </p> 
      </div> 

      <script> 
           var items = document.getElementById("main").getElementsByClassName("target"); 
           for (var i = 0; i < items.length; i++) { 
                var child = document.createElement("p"); 
                var child2 = document.createTextNode("Some text"); 
                child.appendChild(child2); 
                child.setAttribute("style", "color:red; border: 1px solid green;"); 
                items[i].appendChild(child); 
           } 
      </script> 
</body> 
```

How many elements will be red with a green border?

Choose the correct answer

1) 1
2) 2
3) 3
4) 4

#### From Kenn: Don't over think it
