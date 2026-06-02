# Ex08 CAMU Schedule using Bootstrap
## Date:

## AIM:
To design a responsive and visually appealing CAMU Schedule using Bootstrap.

## DESIGN STEPS:
### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Add the Bootstrap CDN link inside the <head> section.

### Step 5:
Insert a table element with Bootstrap table classes.

### Step 6:
Construct the complete table.

### Step 7:
Add a header/footer displaying copyright information.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM :
schedule.html
```
{% load static %}

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CAMU Schedule</title>

    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">

    <style>

        body{
            background: linear-gradient(135deg,#4facfe,#00f2fe);
            min-height:100vh;
        }

        .main-card{
            background:white;
            border-radius:20px;
            box-shadow:0px 10px 25px rgba(0,0,0,0.2);
            overflow:hidden;
        }

        .header{
            background:#0d6efd;
            color:white;
            text-align:center;
            padding:25px;
        }

        .logo{
            width:120px;
            height:120px;
            border-radius:50%;
            background:white;
            padding:5px;
        }

        table{
            text-align:center;
        }

        tbody tr:hover{
            background:#d6ecff;
        }

        .footer{
            text-align:center;
            margin-top:20px;
            color:white;
            font-weight:bold;
        }

    </style>
</head>

<body>

<div class="container mt-5">

    <div class="main-card">

        <div class="header">

            <img src="{% static 'image/image.png' %}" class="logo">

            <h2 class="mt-3">SAVEETHA ENGINEERING COLLEGE</h2>

            <h5>Department of Computer Science</h5>

            <h3>CAMU Schedule</h3>

        </div>

        <div class="p-4">

            <table class="table table-bordered table-striped table-hover">

                <thead class="table-dark">

                    <tr>
                        <th>Time</th>
                        <th>Monday</th>
                        <th>Tuesday</th>
                        <th>Wednesday</th>
                        <th>Thursday</th>
                        <th>Friday</th>
                    </tr>

                </thead>

                <tbody>

                    <tr>
                        <td>9:00 - 10:00</td>
                        <td>Python</td>
                        <td>DS</td>
                        <td>OS</td>
                        <td>AI</td>
                        <td>CN</td>
                    </tr>

                    <tr>
                        <td>10:00 - 11:00</td>
                        <td>DS</td>
                        <td>Python</td>
                        <td>AI</td>
                        <td>CN</td>
                        <td>Lab</td>
                    </tr>

                    <tr>
                        <td>11:00 - 12:00</td>
                        <td>OS</td>
                        <td>AI</td>
                        <td>DS</td>
                        <td>Python</td>
                        <td>Project</td>
                    </tr>

                    <tr class="table-warning">
                        <td colspan="6">
                            <b>LUNCH BREAK</b>
                        </td>
                    </tr>

                    <tr>
                        <td>1:00 - 2:00</td>
                        <td>Lab</td>
                        <td>Project</td>
                        <td>CN</td>
                        <td>DS</td>
                        <td>Seminar</td>
                    </tr>

                    <tr>
                        <td>2:00 - 3:00</td>
                        <td>Placement</td>
                        <td>Sports</td>
                        <td>Library</td>
                        <td>Project</td>
                        <td>Placement</td>
                    </tr>

                </tbody>

            </table>

        </div>

    </div>

    <div class="footer">
        © 2026 CAMU Schedule
    </div>

</div>

</body>
</html>
```


## OUTPUT:

![alt text](<Screenshot 2026-06-02 144327.png>)

## RESULT:
A responsive and visually appealing CAMU Schedule web page using Bootstrap is designed successfully.
