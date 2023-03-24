<!DOCTYPE html>
<html ng-app="wpmCalculator">
  <head>
    <title>WPM Calculator</title>
    <meta charset="UTF-8">
    <meta name="description" content="Words per minute calculator built with HTML, CSS, JavaScript, jQuery and Bootstrap.">
    <meta name="author1" content="Pooja R">
  

    <!--favicon-->
      <link rel="icon" href="favicon.ico" type="image/png" >
    <!--Font Awesome-->
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css">

    <!--Roboto font from Google-->
      <link href='https://fonts.googleapis.com/css?family=Roboto' rel='stylesheet' type='text/css'>

    <!--jQuery-->
      <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>

    <!--Bootstrap-->
      <!-- Latest compiled and minified CSS -->
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">
      <!-- Optional theme -->
      <!--<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap-theme.min.css">-->
      <!-- Latest compiled and minified JavaScript -->
      <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>

    <!--Local stylesheet-->
      <link rel="stylesheet" href="css/styles.css">

    <!--Local script-->
      <script src="js/main.js"></script>

  </head>

  <body>
    <!--header-->
    <div class="jumbotron onesidedropshadow">
      <h1 class="jumbotronText">Get ready.</h1>
      <p class="jumbotronText">Test your typing speed.</p>
    </div>

    <div class="container-fluid">

      <div class="row ">

        <div class="col-md-12 text-center">
          <h2>Click the textbox, and copy the content on the left.</h2>
        </div>

      </div>

      <div class="row">

        <!--generated paragraphs-->
        <div class="lead paragraph col-md-6  blocks border">
        </div>
        <!--textarea-->
        <div class="col-md-6  blocks">
          <div class="form-group ">
            <label for="comment">The timer starts when a key is pressed.</label>
            <button type="button" class="resetBtn btn btn-default"><i class="fa fa-refresh"></i> Reset</button>

            <textarea class="form-control" rows="13" id="userInput" onkeypress="CallBoth(event)" onkeydown="BackSpace(event)"></textarea>
            <!--alert-->
            <div class="alert alert-danger alert-dismissible text-center" role="alert">
              <button type="button" class="close" data-dismiss="alert" aria-label="Close"><span aria-hidden="true">&times;</span></button>
              <strong>Warning!</strong> The timer is still running. You must finish typing all of the content!
            </div>

          </div>

        </div>

      </div>

      <!--footer-->
      <div class="row">
        <div class="col-md-12">
          <footer class="footer">
            <div class="container">
              <p class="text-center">By Pooja R.</p>
            </div>
          </footer>
        </div>
      </div>

    </div>
  </body>

</html>
