# Ex04 Places Around Me
## Date: 

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        
        img{
            margin-left: 20%;
            width: 800px;
            height: 400px;
        }
    </style>
</head>
<script>
    function coordinate(event){
        let x =event.clientX;
        let y=event.clientY;
        document.getElementById("X").value=x;
        document.getElementById("Y").value=y;
    }
</script>
<body>
    
    <img src="Screenshot (5).png" width="600" height="230" usemap="#MapNew" onmousemove="coordinate(event)" />
    <map name="MapNew" >
        
        <area shape="rect" coords="96,101,100,30" href="https://www.apolloartsandsciencecollegechennai.ac.in/courses.aspx" title="Appolo arts ands science"/>
        <area shape="rect" coords="600,240,140,190" href="https://www.saveetha.ac.in/" title="Savetha engineering college"/>
        <area shape="rect" coords="475,245,660,220" href="https://dmice.ac.in/" title="DMI college of engineering"/>

        <area shape="rect" coords="880,160,460,95" href="https://www.pleasantdays.in/" title="pleasant days resort"/>


    </map>   <br/>
    X-coordinate <input type="text" id="X"/> <br/>
    Y-coordinate<input type="text" id="Y"/> 
</body>
</html>




## OUTPUT
![alt text](<../Screenshot (6).png>)
![alt text](<../Screenshot (10).png>)
![alt text](<../Screenshot (11).png>)
![alt text](<../Screenshot (7).png>)
![alt text](<../Screenshot (9).png>)


## RESULT
The program for implementing image maps using HTML is executed successfully.
