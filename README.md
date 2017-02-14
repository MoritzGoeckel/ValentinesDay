# Valentines Day Card
This is a little website I made for valentines day.

[See the demo here](http://moritzgoeckel.com/ValentinesDay/)

## Change it
If you want to customize the website you can follow these steps:

### Change the picture.jpg
You should choose one that is dark on the edges and has some space on the left.

### Change the Names in the index.html (Line 7 and 9)
``` html
<span class="leftText">
    Moritz<br /> <---- Here
    <span class="love">loves</span><br />
    Christine<br /> <---- And here
    <span class="since">since</span><br />
    ...
</span>
```

## Change the date in the index.html (Line 22)
``` javascript
function getLoveTime() {
    //14. April 2016
    var time = Date.now() - new Date(2016, 4 - 1, 14, 0, 0, 0, 0).getTime(); <---- Here
    time = new Date(time);
    return time / (1000*60*60*24);
}
```