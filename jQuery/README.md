#### 1. Ajax

Łączenie się z serwerem, pobranie danych i wypisanie ich w konsoli:

```
$.ajax({
  url: "XXXX",
  method: "GET",
  dataType: "json"
})
  .done(function(response) {
    console.log(response);
  });
```
Gdzie XXXX to adres serwera.
