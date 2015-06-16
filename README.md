# angularTraning
DIving into Angular for the first time
<!doctype html>
<html lang="en" ng-app="phonecatApp">
<head>
  <meta charset="utf-8">
  <title>Google Phone Gallery</title>
  <link rel="stylesheet" href="bower_components/bootstrap/dist/css/bootstrap.css">
  <link rel="stylesheet" href="css/app.css">
  <script src="bower_components/angular/angular.js"></script>
  <script src="js/controllers.js"></script>
</head><h3>Hello {{name}}</h3>
<body ng-controller="PhoneListCtrl">

  <ul>
    <li ng-repeat="phone in phones">
      <span>{{phone.name}}</span>
      <p>{{phone.snippet}}</p>
      <p>{{phone.price}}</p>
    </li>
    <p>Total number of phones: {{phones.length}}</p>
  </ul>
  
  <table style="width:100%">
  <tr><th ng-repeat="x in [0, 1, 2, 3, 4, 5, 6, 7]">row number {{x}}</th></tr>
  <tr ng-repeat="i in [0, 1, 2, 3, 4, 5, 6, 7]">
  <td ng-repeat="j in [0, 1, 2, 3, 4, 5, 6, 7]">{{i+j}}</td>
  </tr>

</table>

</body>
</html>

