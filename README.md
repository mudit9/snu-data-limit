# snu-data-limit
A small script that calculates the data you have downloaded since the last wednesday


[I'm a reference-style link][Arbitrary case-insensitive reference text]

[arbitrary case-insensitive reference text]: javascript:(function()%7Bvar%20sum%20%3D%200.0%3Bvar%20date_n%20%3D%20new%20Date()%3Bvar%20currentTime%20%3D%20date_n%3Bvar%20currentDay%20%3D%20currentTime.getDay()%3Bvar%20wednesday%20%3D%203%3Bvar%20daysBack%2C%20pastDate%3Bif(currentDay%20%3E%20wednesday)%7BdaysBack%20%3D%20currentDay%20-%20wednesday%3B%7Delse%7BdaysBack%20%3D%20(7%20-%20wednesday)%20%2B%20currentDay%3B%7Dlast_wednesday%20%3D%20new%20Date(date_n.getFullYear()%2Cdate_n.getMonth()%2C%20date_n.getDate()%20-%20daysBack)%3Bconsole.log(last_wednesday)%3Bfor%20(i%20%3D%2018%3B%20i%20%3C%20document.getElementsByTagName('tr').length%20-%204%3B%20i%2B%2B)%7Bd%20%3D%20parseFloat(document.getElementsByTagName('tr')%5Bi%5D.childNodes%5B6%5D.innerHTML.split('%20')%5B0%5D)%3Bdate%20%3D%20new%20Date(document.getElementsByTagName('tr')%5Bi%5D.childNodes%5B3%5D.innerHTML%20%2B%20%22%2C%202015%22)%3Bif(date%20%3E%20last_wednesday)%7Bsum%20%2B%3D%20d%3B%7D%7Dalert(%22downloaded%20%3D%20%22%20%2B%20sum)%7D)()