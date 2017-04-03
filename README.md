# nepali-calendar-api
A nepali calendar api conisiting of both AD and BS dates with 'tithi' and other Nepal specific info.

The api is hosted as static json file in github (inside the api folder).

# demo
https://bibhuticoder.github.io/nepali-calendar-api/api/2073.json

# usage
```javascript
//request
var year = "calendar of this year"; //1970 to 2074
$.ajax({
  method: "GET",
  url : "https://bibhuticoder.github.io/nepali-calendar-api/api/"+year+".json",
  success:function(d){
    console.log(d);
  }
});

//response
{
  "Baisakh":[
    {
      "np": "31", //Date in BS
      "en": "14", // Date in AD
      "tithi": " तृतीया ", // nepali 'tithi'
      "event": "टोखा चण्डेश्वरी रथयात्रा", //name of the event that day
      "day": "sun", //day of the week
      "specialday": false, //day with special kind of event
      "holiday": false //National holiday
    
    },
    ...,
    ...
  ],
  "Jestha" :[...],
  "..." : [...]
}
```

# Apps using the api
- Nepali-calendar : https://bibhuticoder.github.io/nepali-calendar
