ngRadialGauge
=============

Angular.js Radial Gauge

![alt tag](https://raw.github.com/stherrienaspnet/D3-Radial-Gauge/master/D3RadialGauge.png)

Here is a sample usage:
``` 
<body ng-app="myApp">
    <div ng-controller="RadialGaugeCtrl">
        <div style="width: 200px;" ng-radial-gauge ranges="ranges" value="value" value-unit="unit" 
        precision="precision" lower-limit="lowerLimit" upper-limit="upperLimit"></div>
    </div>
</body>

app.controller('RadialGaugeCtrl', ['$scope', function ($scope) {
    $scope.value = 1.5;
    $scope.upperLimit = 6;
    $scope.lowerLimit = 0;
    $scope.unit = "kW";
    $scope.precision = 2;
    $scope.ranges = [
        {
            min: 0,
            max: 1.5,
            color: '#DEDEDE'
        },
        {
            min: 1.5,
            max: 2.5,
            color: '#8DCA2F'
        },
        {
            min: 2.5,
            max: 3.5,
            color: '#FDC702'
        },
        {
            min: 3.5,
            max: 4.5,
            color: '#FF7700'
        },
        {
            min: 4.5,
            max: 6.0,
            color: '#C50200'
        }
    ];
}]);
```
