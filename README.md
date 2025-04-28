# Ex.08 Design of Interactive Image Gallery
## Date:

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        #flexbox
        {
            
            padding: 100px;
            background-color: aliceblue;
        }
        #container1
        {
            
            display: flex;
            background-color: aliceblue;
            gap: 20px;
            justify-content: center;
            padding: 10px;
            padding: 40px;
            box-shadow: 0 2px 3px;
        }
        
        .img
        {
            height: 150px;
            width: 250px;
            
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(26, 24, 24, 0.5);
            position: fixed;
            width: 100%;
            
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        #title
        {
            background-color:paleturquoise;
            font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
            border-radius: 10px;
            width: 500px;
            transition: 0.5s;
            box-shadow: 0 3px 10px;
            position: absolute;
            top: 20px;
            padding: 20px;
            left: 500px;
        }
        #title:hover{
            transform: scale(1.1);
        }
    </style>
</head>
<body>
    <section id="image">
            <img src=" " alt="" id="display" onclick="closes()" style="height: 900px; width: auto; border: 10px inset black;">
    </section>
<div id="flexbox">

    <h1 align="center" ><span id="title">Photo Gallery</span></h1>

    <div id="container1">
        <div class="divs"><img class="img" src="panda.jpg" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="giraffee.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="nature-3162233_960_720.jpg"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="tiger.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs" ><img class="img" src="anil.jpg" onclick="opens(this.src)"   alt=""></div>
    </div>
    
</div>

    
    

    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/cf982b67-e802-4d99-bc03-4bf523cddfc4)

![tiger scr](https://github.com/user-attachments/assets/f682df36-3cd8-45de-97e2-f41e0be545df)

![pap scr](https://github.com/user-attachments/assets/20639fa2-3a0b-49f0-b005-d418caf57d3d)

![panda scr](https://github.com/user-attachments/assets/1cf75fe0-f34d-4b7b-aa85-8bd9547b51ca)

![giraffee scr](https://github.com/user-attachments/assets/c97cfcdf-d70e-41b2-9cec-02a2a5e331ed)

## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
