# Design a Website for Server Side Processing

## AIM:
To design a website to perform mathematical calculations in server side.

## DESIGN STEPS:

### Step 1:
Clone into the repository named 'serversideprocessing' and create a project named 'myfirstproject'.

### Step 2:
Startapp 'myfirstapp'.Create a folder named 'templates' under which all html files are stored.

### Step 3:
Make the necessary changes in the settings.py and add codes in urls.py and views.py which enables the operation to take place.

### Step 4:
Under templates and myfirstapp, create a html file named math.html and write the required html code for the website.

### Step 5:
Then makemigrations and run the server to get the output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
    <head>
        <style type="text/css">
        body{
            background-color: blueviolet;
        }
        .color1{
            background-color: #FF00B6;
        }
        .color2{
            background-color: #C800FF;
        }
        .color3{
            background-color: #FF0037;
        }
        #calculation{
            width:750px;
            height:300px;
            margin-left: auto;
            margin-right: auto;
            margin-top: 200px;
            margin-bottom: auto;
            border-width: 5px;
            border-color: #FF0037;
            border-style: groove;
        }
        .block{
            text-align:center;
            width:375px;
            height:40px;
            margin-top: auto;
            margin-bottom: auto;
            margin-left: auto;
            margin-right: auto;
            background-color: #FF00B6;
        }
        </style>
    </head>
    <body>
        <div id="calculation" class="color2" align="center">
        <h1>Volume of Cuboid</h1>
        <form method="POST" action="/math/">
            {%csrf_token%}
            <div class="block">
            <label for="length">Length</label>
            <input type="text" name="length" id="length" value="{{ length }}"/>
            </div>
            <div class="block">
            <label for="breadth">Breadth</label>
            <input type="text" name="breadth" id="breadth" value="{{ breadth }}"/>
            </div>
            <div class="block">
            <label for="height">Height</label>
            <input type="text" name="height" id="height" value="{{ height }}"/>
            </div>
            <div class="block">
            <input type="submit" value="Calculate volume"/>
           </div>
           <div class="block">
            <label for="volume">Volume</label>
            <input type="text" name="volume" id="volume" value="{{ volume }}"/>
            </div>
        </form>
        </div>
    </body>
</html>
```
## OUTPUT:
### Home Page:
![HOMEPAGE](./homevolume.png)

### Calculations:

![AREAOUTPUT](./value.png)

## Result:
Calculations are performed correctly as per the given inputs.
