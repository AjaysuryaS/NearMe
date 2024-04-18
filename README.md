# Ex04 Places Around Me
## Date: 
18/04/23
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
    <title>Image Map</title>
</head>
<body>
    <IMG src="map.png" width="1000" height="430" usemap="#MapNew" onmousemove="coordinate(event)"></IMG>
    <MAP name="MapNew">

        <AREA shape="RECT" coords="388,288,414,292" href="https://nithyahospital.com/" Title="Nithya Hospital">
        <AREA shape="RECT" coords="414,286,441,292" href="https://www.esic.gov.in/hospitals" Title="ESI hospital">
        <AREA shape="RECT" coords="504,397,500,388" href="http://dhineshhospitals.com/contact.html" Title="Dinesh Hospital">
        <AREA shape="RECT" coords="482,304,536,314" href="https://www.healthdoc.in/vellore/hospital/sankari-hospital-293956" Title="Sankari hospital">
        <AREA shape="RECT" coords="543,192,500,200" href="https://www.cmch-vellore.edu/" Title="cmc vellore">

    </MAP><br>
    X-coordinate <input type="text" id="X"><br>
    Y-coordinate <input type="text" id="Y">

    <script>
        function coordinate (event) {
        let x = event.clientX;
        let y = event.clientY;
        document.getElementById("X").value = x
        document.getElementById("Y").value = y
        } 
    </script>

</body>
</html>

## OUTPUT

![Screenshot 2024-04-18 135207](https://github.com/AjaysuryaS/NearMe/assets/114158396/af9e2856-fdd8-42b8-bf26-c4a54b70d03f)
![Screenshot 2024-04-18 135222](https://github.com/AjaysuryaS/NearMe/assets/114158396/99a3e142-118f-4b9f-8079-6e3a9efd2318)
![Screenshot 2024-04-18 135234](https://github.com/AjaysuryaS/NearMe/assets/114158396/d3e54f5e-afa8-4b67-b798-adae3a80e88f)
![Screenshot 2024-04-18 135250](https://github.com/AjaysuryaS/NearMe/assets/114158396/f09de070-df68-48eb-987f-c5665de4ce4c)
![Screenshot 2024-04-18 135305](https://github.com/AjaysuryaS/NearMe/assets/114158396/61468748-364d-4eac-977a-de70a6279e6c)

## RESULT
The program for implementing image maps using HTML is executed successfully.
