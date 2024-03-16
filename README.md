Task.1:- Create an image gallery using Grid.  <br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .container{
            height: 100vh;
            display: grid;
            grid-template-areas:
                'photo-1 photo-1 photo-1 photo-1 photo-2 photo-2'
                'photo-3 photo-3 photo-4 photo-4 photo-6 photo-6'
                'photo-3 photo-3 photo-5 photo-5 photo-6 photo-6';
                gap: 10px;       
        }
        .item{border-radius:20px;
        }

        .photo-1{
            grid-area:photo-1;
            background-image: url("https://images.pexels.com/photos/276267/pexels-photo-276267.jpeg?");
            background-size: cover;
        }
        .photo-2{
            grid-area:photo-2;
            background-image: url("https://images.pexels.com/photos/159045/the-interior-of-the-repair-interior-design-159045.jpeg?");
            background-size: cover;
        }
        .photo-3{
            grid-area:photo-3;
            background-image: url("https://images.pexels.com/photos/4033148/pexels-photo-4033148.jpeg?");
            background-size: cover;
        }
        .photo-4{
            grid-area:photo-4;
            background-image: url("https://images.pexels.com/photos/34299/herbs-flavoring-seasoning-cooking.jpg?");
            background-size: cover;
        }
        .photo-5{
            grid-area:photo-5;
            background-image:url("https://images.pexels.com/photos/6074935/pexels-photo-6074935.jpeg?");
            background-size:cover;
        }
        .photo-6{
            grid-area:photo-6;
            background-image:url("https://images.pexels.com/photos/4210610/pexels-photo-4210610.jpeg?");
            background-size:cover;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="item photo-1"></div>
        <div class="item photo-2"></div> 
        <div class="item photo-3"></div> 
        <div class="item photo-4"></div> 
        <div class="item photo-5"></div>
        <div class="item photo-6"></div> 
      </div>
</body>
</html>

Task.2:- Write code to arrange containers with texts A,B,C and D as shown in the project.   <br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        .container{
            height: 100vh;
            display: grid;
            grid-template-areas:
                'photo-1 photo-1 photo-1 photo-1 photo-4 photo-4'
                'photo-2 photo-2 photo-3 photo-3 photo-4 photo-4'
                'photo-2 photo-2 photo-3 photo-3 photo-4 photo-4';
                gap: 10px;      
                padding: 40px; 
        }
        .item{border-radius:20px;
            padding: 50px;
            font-size: 400%;
            display: flex;
            align-items: center;
            justify-items: center;
        }
        .photo-1{
            grid-area:photo-1;
            background-color:pink;
        }
        .photo-2{
            grid-area:photo-2;
            background-color:pink;
        }
        .photo-3{
            grid-area:photo-3;
            background-color:pink;
        }
        .photo-4{
            grid-area:photo-4;
            background-color:pink;
        } 
    </style>
</head>
<body>
    <div class="container">
        <div class="item photo-1"> A</div>
        <div class="item photo-2">C</div> 
        <div class="item photo-3">D</div> 
        <div class="item photo-4">B</div>  
      </div>
</body>
</html>

Task.3:-Explain the use of grid-auto-row and grid-auto-column using code examples.   <br>
 Answer:- grid-auto-row and grid-auto-column are properties used in CSS Grid Layout to specify the size of rows and columns that are created implicitly to accommodate additional content beyond what is defined in the grid template.

Here's how you can use grid-auto-row and grid-auto-column with code examples:

