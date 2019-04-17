# DIGITAL GODS: SUNSET
Creando un atardecer

![digitalGods](https://github.com/nicolasbaez/mad021/blob/master/descarga.png)

1. gameDev.htm
```html
<html>
    <script src="p5.js">
        //Descarga: https://cdnjs.cloudflare.com/ajax/libs/p5.js/0.8.0/p5.js
    </script>
    <script src="p5.dom.js">
        //Descarga: https://raw.githubusercontent.com/lmccart/p5.js/master/lib/addons/p5.dom.js
    </script>
    <script src="digitalGods.js">
        //Nuestro juego de video
    </script>
    <body style="margin:0;">
    </body>
</html>
```
2. digitalGods.js
```html
function setup() {
 createCanvas(window.innerWidth,window.innerHeight);
 background(0);
}
function atardecer(){
    for(var i=height;i>0;i--){
    //rr,gg,bb
    stroke(map(i,height,0,255,0),map(i,height,0,102,0),map(mouseX,0,width,0,255));
    line(0,i,width,i);
  }
}
function draw() {
  atardecer();
}
```
