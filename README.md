# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title> AR Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/icon/icon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        AR Private Limited
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 AR Private Limited, Developed by Arun.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/build.jpg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### people.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="peoplecontent">
    <h1>Our Crew</h1>
    <div class="crewmembers">
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/HOD.jpg" alt="member image" width="200" height="200">
            </div>
            <div class="membername">OBED OTTA</div>
            <div class="designation">C.E.O </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/JOSHAN.jpg" alt="member image" width="200" height="200">
            </div>
            <div class="membername">JOSHAN ATHANESIOUS</div>
            <div class="designation">FRONTEND DEV</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/Aravind1.png" alt="member image" width="200" height="200">
            </div>
            <div class="membername">ARAVIND</div>
            <div class="designation">TECHNICAL TEAM</div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/Arjun1.jpg" alt="member image" width="200" height="200">
            </div>
            <div class="membername">ARJUNRAJ</div>
            <div class="designation"> R & D HEAD </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/Vivek.jpg" alt="member image" width="200" height="200">
            </div>
            <div class="membername">VIVEK </div>
            <div class="designation"> DESIGN TEAM </div>
        </div>
        <div class="crewmember">
            <div class="memberimage">
                <img src="/static/img/ppl/Arun.jpeg" alt="member image" width="200" height="200">
            </div>
            <div class="membername">ARUNRAJ</div>
            <div class="designation"> MARKETING HEAD </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/mboard.jpg"  alt="product image">
            </div>
            <div class="itemname">MSI Z490-A PRO ATX Gaming Motherboard</div>
            <div class="itemprice">Price: Rs.16,000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/ssd.jpeg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop SSD</div>
            <div class="itemprice">Price: Rs.10,000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/ryzen.jpg"  alt="product image">
            </div>
            <div class="itemname">AMD Ryzen 3 3200G </div>
            <div class="itemprice">Price: Rs.10,000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/ram.jpg"  alt="product image">
            </div>
            <div class="itemname">HyperX Fury 8GB 3200MHz DDR4</div>
            <div class="itemprice">Price: Rs.3500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/km.jpg"  alt="product image">
            </div>
            <div class="itemname">WisFox 2.4G Full-Size Slim Thin Wireless Keyboard and Mouse</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/acer.jpg"  alt="product image">
            </div>
            <div class="itemname">Acer Predator 21X</div>
            <div class="itemprice">Price: Rs.8,00,000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/gc.jpg"  alt="product image">
            </div>
            <div class="itemname">Gigabyte NVIDIA GeForce GT 710 2 GB DDR3</div>
            <div class="itemprice">Price: Rs.3000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/cd.jpg"  alt="product image">
            </div>
            <div class="itemname">Rts External CD Drive</div>
            <div class="itemprice">Price: Rs.1500.00</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/fb.jpg"  alt="product image">
            </div>
            <div class="itemname">Fitbit Versa Smart Watch</div>
            <div class="itemprice">Price: Rs.12,000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/products/rp.jpg"  alt="product image">
            </div>
            <div class="itemname">Raspberry Pi 4 8GB RAM</div>
            <div class="itemprice">Price: Rs.7500.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### contactus.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="contactuscontent">
        <div class="contactbox">
            <div>
                <img src="/static/img/contact.png" alt="contactusimg">
            </div>
        </div>
        <hr/>
        <div class="contactemail"><h1>Email: arun@ar.ac.in</h1></div>
        <div class="contactphone"><h2>Phone: +91-7200742352</h2></div>
        <div class="contactphone"><h2>Address: © AR pvt,Silicon valley, Microsoft, Google</h2></div>
        <hr/>
    </div>

{% endblock %}
```
## OUTPUT:
![output](./static/img/output/o1.png)

![output](./static/img/output/o2.png)

![output](./static/img/output/o3.png)

![output](./static/img/output/o4.png)

## CODE VALIDATION REPORT:
![output](./static/img/report/v1.png)

![output](./static/img/report/v2.png)

![output](./static/img/report/v3.png)

![output](./static/img/report/v4.png)

## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://arun.student.saveetha.in:8000/. HTML code is validated.