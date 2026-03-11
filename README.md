# Ex.04 Design a Website for Server Side Processing
## Date:11.03.2026

## AIM:
To create a web page to calculate total bill amount with GST from price and GST percentage using server-side scripts.

## FORMULA:
Bill = P + (P * GST / 100)
<br> P --> Price (in Rupees)
<br> GST --> GST (in Percentage)
<br> Bill --> Total Bill Amount (in Rupees)

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create a HTML file to implement form based input and output.

### Step 5:
Create python programs for views and urls to perform server side processing.

### Step 6:
Receive input values from the form using request.POST.get().

### Step 7:
Calculate the total bill amount (including GST).

### Step 8:
Display the calculated result in the server console.

### Step 9:
Render the result to the HTML template.

### Step 10:
Publish the website in Localhost.

## PROGRAM:
```

gst.html

<html>
   <head>
      <title>GST Bill Calculator</title>

    <style>
    .box {
            width:480px;
            height:300px;
            border:ridge 3px black;
            padding:10px;
            position:fixed;
            top:200px;
            left:550px;
            background-color:silver;
            text-align:center;
    }
    </style>

   </head>

<body bgcolor="teal">

    <div class="box">
<h1>Total Bill  with GST</h1>
<h3>RAMESH JAISURYA (25005800)</h3>
<form method="POST">
{% csrf_token %}

<div>
<label>Price : </label>
<input type="text" name="price" required>
</div><br>
<div>
<label>GST :</label>
<input type="text" name="gst" required>
</div><br>
<div>
<input type="submit" value="Calculate">
</div><br>
<div>
<label>Total Bill (₹)</label>
<input type="text" value="{{bill}}">
</div>

</form>
</div>
</body>
</html>
    
```




## OUTPUT - SERVER SIDE:
![alt text](<Screenshot (95).png>)

## OUTPUT - WEBPAGE:

![alt text](<Screenshot (97).png>)


## RESULT:
The a web page to calculate total bill amount with GST from price and GST percentage using server-side scripts is created successfully.
