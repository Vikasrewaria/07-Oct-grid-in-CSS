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
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    .grid-container {
      display: grid;
      grid-template-columns: 100px 100px;     
      grid-auto-rows: 50px;
      grid-auto-columns: 50px; 
      gap: 5px;
    }    
    .grid-item {
      background-color: lightblue;
      border: 1px solid black;
    }
  </style>
</head>
<body>
   <div class="grid-container">
    <div class="grid-item">1</div>
    <div class="grid-item">2</div>
    <div class="grid-item">3</div>
    <div class="grid-item">4</div>
    <div class="grid-item">5</div>
    <div class="grid-item">6</div>
    <div class="grid-item">7</div>
    <div class="grid-item">8</div>
    <div class="grid-item">9</div>
    <div class="grid-item">10</div>
  </div>
</body>
</html>

The .grid-container class sets up a grid-container with explicit columns of 100 pixels each.
grid-auto-rows is set to 50 pixels, meaning any rows created implicitly to accommodate additional content will have a height of 50 pixels.
grid-auto-columns is set to 50 pixels, meaning any columns created implicitly to accommodate additional content will have a width of 50 pixels.

When you add more items than the explicitly defined grid can accommodate, additional rows and columns are created implicitly. These implicit rows and columns will have a size defined by grid-auto-rows and grid-auto-columns, respectively.

Task.4:-Write CSS to show numbers as shown in the figure, without altering the below html code.
<br>
Answer:- <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style>
    .grid-container {
      border: 1px solid black ;
      gap: 20px;
      padding:50px;
      display: grid;
      grid-template-columns: repeat(6,1fr);
      
    }
    .box{
      height: 150px;
    border: 2px solid black ;
    border-radius:10px;
    gap:2px;
    font-size: 150%;
    }
    .box-1{
      background-color: grey;
      order: 7;
    }
    .box-2{
      background-color:rgb(246, 240, 240) ;
      order:8;
    }
    .box-3{
      background-color: grey;
      order:1;
    }
    .box-4{
      background-color: rgb(246, 240, 240);
      order:2;
    }
    .box-5{
      background-color: grey;
      order: 3;
    }
    .box-6{
      background-color: rgb(246, 240, 240);
      order:4;
    }
    .box-7{
      background-color:grey;
      order:5;
    }
    .box-8{
      background-color:rgb(246, 240, 240);
      order:6;
    }
    </style>
</head>
<body>
   <div class="grid-container">
    <div class="box box-1">1</div>
    <div class="box box-2">2</div>
    <div class="box box-3">3</div>
    <div class="box box-4">4</div>
    <div class="box box-5">5</div>
    <div class="box box-6">6</div>
    <div class="box box-7">7</div>
    <div class="box box-8">8</div>
  </div>
</body>
</html>

Task.5:-Explain the difference between justify-items and justify-self using code examples.
Answer:-
In CSS Grid Layout, both justify-items and justify-self are properties used to align grid items along the inline (horizontal) axis within their grid cells. However, they operate at different levels:

justify-items: This property is used to align all the grid items within the grid container along the inline axis. It applies to the whole grid container.

justify-self: This property is used to align individual grid items within their respective grid cells along the inline axis. It applies to individual grid items.

Here's an example to demonstrate the difference between justify-items and justify-self:
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>justify-items vs justify-self Example</title>
<style>
  .grid-container {
    display: grid;
    grid-template-columns: repeat(3, 100px);
    justify-items: center; 
    gap: 10px;
  }
  
  .grid-item {
    background-color: lightblue;
    border: 1px solid black;
  }
  
  .item-2 {
    justify-self: end; 
  }
</style>
</head>
<body>

<div class="grid-container">
  <div class="grid-item">1</div>
  <div class="grid-item item-2">2</div>
  <div class="grid-item">3</div>
  <div class="grid-item">4</div>
  <div class="grid-item">5</div>
  <div class="grid-item">6</div>
</div>

</body>
</html>


