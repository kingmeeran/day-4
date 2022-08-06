# day-4
1.COMPARE 2 JSON PROPERTIES

var obj = {name: "jhon", age: 5}; var names= JSON.stringify(obj); console.log(names);

var obj = {age: 5, name: "jhon"}; var names= JSON.stringify(obj); console.log(names);

2.REST COUNTRIES DISPLAY ALL FLAGS

var request=new XMLHttpRequest();

request.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json"); 
request.send();
request.onload=function(){
var result=JSON.parse(request.response); 
console.log(result); 
for(var i=0;i<result.length;i++){
console.log(result[i].flag);

3.REST COUNTRIES DISPLAY COUNTRY NAME,POPULATION,REGION,SUB-REGION

var request=new XMLHttpRequest();

request.open("GET","https://raw.githubusercontent.com/rvsp/restcountries-json-data/master/res-countries.json");
request.send(); 
request.onload=function(){ 
var result=JSON.parse(request.response);
console.log(result);
for(var i=0;i<result.length;i++){ 
console.log(result[i].name); 
console.log(result[i].population);
console.log(result[i].region)
; console.log(result[i].subregion);
}}
