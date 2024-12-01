<!DOCTYPE html>
<html lang="en">
  <head>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.3.1/p5.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.3.1/addons/p5.sound.min.js"></script>
    
    <meta charset="utf-8" />
  <title>There is a fire,graphic</title>
  </head>
  <body>
  <script>
  function setup() {
  createCanvas(720,400);
  background('aqua');
  x=width/2;
  y=height;
}

function draw() {
 // draw a circle 
  noStroke();
  fill('lightgray');
  ellipse(x,y,24,24);
  
  //jiggling horizontal axis
  x=x + random(-1,1);
  
  //moving
   y=y-1;
  
  //reset to bottom
  if(y < 0){
    y=height;
  
  stroke(255,0,0);
  fill(0,210,241);
  rect(30,380,40,50,10);//building1
  
  stroke(0,0,0);
  fill(10,30,240);
  rect(50,350,70,50);//building2
  
  stroke(0,0,0);
  fill(0,220,100);
  rect(100,320,60,100,20);//building3
  
  stroke(0,0,0);
  fill(100,100,100);
  rect(160,360,100,200,10);//building4
  }
} 
</script>
</body>

</html>
  
