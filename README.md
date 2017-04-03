# nepali-calendar-api
A nepali calendar api conisiting of both AD and BS dates with tithi and other Nepal specific info.

The api is hosted as static json file in github (inside the api folder).

# usage
```javascript
//to access the api
var year = "calendar of this year"; //1970 to 2074
$.ajax({
  method: "GET",
  url : "https://bibhuticoder.github.io/nepali-calendar-api/api/"+year+".json",
  success:function(d){
    console.log(d);
  }
});
```

# demo
https://bibhuticoder.github.io/nepali-calendar
