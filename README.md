<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
  <style> h1 {
    color: red;
}

.add_btn {

    text-align: center;
    margin-top: 6px;
}

.add_btn .red_btn {
    background-color: #ffcccc;
    border-radius: 6px;
    border-color: #ff6767;
}

.add_btn .blue_btn {
    background-color: #d5ccff;
    border-radius: 6px;
    border-color: #8867ff;
}

.add_btn .green_btn {
    background-color: #ccffd1;
    border-radius: 6px;
    border-color: #67ff8a;
}

.add_btn .yellow_btn {
    background-color: #f8ffcc;
    border-radius: 6px;
    border-color: #f7ff67;
}

.title {
    
    /* padding: 2px; */
    text-align: center;
    height: 50px;
    width: 100px;
    
   
    margin-top: 2px;
}
.title .red_box{
    background-color: #ff946a;
    border: solid black 1px;
    border-radius: 4px;
}
.title .yellow_box{
    background-color: #ffff6a;
    border: solid rgb(0, 0, 0) 1px;
    border-radius: 4px;
}
.title .blue_box{
    background-color: #766aff;
    border: solid black 1px;
    border-radius: 4px;
}
.title .green_box{
    background-color: #6aff80;
    border: solid black 1px;
    border-radius: 4px;
}

.close_btn {
    float: right;
    background: red;
    padding: 2px;
    cursor: pointer;
    text-align: center;
    font-size: 12px;
    border-radius: 3px;
    padding-right: 3px;
    padding-left: 3px;
}</style>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet"
    integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">

</head>

<body>
  <h1>My Task</h1>
  <div class="row">
    <div class="col-sm-3">
      <div class="card">
        <div class="add_btn"><span>Yellow</span> <button class="yellow_btn">Add</button></div>
        <div class="card-body">
          <div class="title">
            <div class="yellow_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
          <div class="title">
            <div class="yellow_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card">
        <div class="add_btn"><span>Red</span> <button class="red_btn">Add</button></div>
        <div class="card-body">
          <div class="title">
            <div class="red_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
          <div class="title">
            <div class="red_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card">
        <div class="add_btn"><span>Blue</span> <button class="blue_btn">Add</button></div>
        <div class="card-body">
          <div class="title">
            <div class="blue_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
          <div class="title">
            <div class="blue_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
        </div>
      </div>
    </div>
    <div class="col-sm-3">
      <div class="card">
        <div class="add_btn"><span>Green</span> <button class="green_btn" onclick="add_green_box()">Add</button></div>
        <div class="card-body">
          <div class="title" id="green_container">
            <div class="green_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
          <div class="title">
            <div class="green_box"><span class="close_btn">X</span><br><span>title</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-w76AqPfDkMBDXo30jS1Sgez6pr3x5MlQ1ZAGC+nuZB+EYdgRZgiwxhTBTkF7CXvN"
    crossorigin="anonymous"></script>
    <script src="assets/js/vendor/jquery-1.12.0.min.js"></script>
  <script>
    function add_green_box() {
var html=`<div class='title'><div class='green_box'><span class='close_btn'>X</span><br><span>title</span></div></div>`;
        jQuery("#green_container").append(html);
        
    }
  </script>
</body>

</html>
