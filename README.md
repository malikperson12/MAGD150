//Lab 1
# MAGD150

function setup() { createCanvas(400, 400); }
function draw() { background(75); 
                 rect(50, 195, 100, 200); 
                 // rect(x, y, width, height) 
                 rect(150, 195, 100, 200); // rect(x, y, width, height) 
                 line(180, 350, 180, 395); // line(x1, y1, x2, y2) Left line 
                 line(220, 350, 220, 395); // line(x1, y1, x2, y2) Right Line 
                 line(180, 350, 220, 350); // line(x1, y1, x2, y2) Top line
                 line(200, 350, 200, 395); // line(x1, y1, x2, y2) Middle Line 
                 strokeWeight(3.0); 
                 strokeCap(SQUARE); 
                 ellipse(200,250,75,75); 
                 noFill(); ellipse(100,250,75,75); 
                 point(195, 375); // point(x, y) door knob left point(205, 375); // point(x, y) door knob right
                }
                
                -----------------------------------------------------------------------------------------------------------------------------------------
//Lab 2                
                
let i = 0; 
  
function setup(){
  createCanvas(400, 400);
  rectMode(CENTER);
  print(5+8.37*3);
print(80.8-4/2);
  print(min(3,7) + max(4,8));
  

  
}
function draw(){
  
  background(150);
  
  if (i==1){
   //light blue bubble
    
    fill(0, 300, 400);
    
    let x1 = map(mouseX, 0, width, 150, 250, true);
      let x2 = map(mouseY, 0, width, 150, 250, true);
      let x3 = map(pmouseX, 0, width, 150, 250, true);
      
    
  ellipse(x1, 200, 250, 250);
  ellipse(x2, 200, 225, 225);
    ellipse(x3, 125, 25, 25);
    
     text(nf(3.3),55,55);
    
  }
  
  
  else if (i > 1){
    //medium blue bubble
    
    fill(0, 200, 400);
    
      let x1 = map(mouseX, 0, width, 150, 250, true);
      let x2 = map(mouseY, 0, width, 150, 250, true);
      let x3 = map(pmouseX, 0, width, 150, 250, true);
      
    
  ellipse(x1, 200, 250, 250);
  ellipse(x2, 200, 225, 225);
    ellipse(x3, 125, 25, 25);
    
      text(nf(5.5),55,55);
  
  }
  
  
  else if (i < 1){
    //dark blue bubble
    
    
    fill(0, 100, 400);
      
  let x1 = map(mouseX, 0, width, 150, 250, true);
  let x2 = map(mouseY, 0, width, 150, 250, true);
  let x3 = map(pmouseX, 0, width, 150, 250, true);
      
    
  ellipse(x1, 200, 250, 250);
  ellipse(x2, 200, 225, 225);
  ellipse(x3, 125, 25, 25);
    
     text(nf(7.7),55,55);
    
  }

  
}

------------------------------------------------------------------------------------------------------
//Lab 3


function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(51);
  
  noStroke();
colorMode(HSB, 400);
for (let i = 0; i < 400; i++) {
  for (let j = 0; j < 400; j++) {
    stroke(i, j, 400);
    point(i, j);
  }
}
  
  noStroke();
colorMode(RGB, 300);
for (let i = 0; i < 300; i++) {
  for (let j = 0; j < 300; j++) {
    stroke(i, j, 0);
    point(i, j);
  }
}
 
  let c = color(400, 190, 0);
fill(c);
noStroke();
ellipse(100, 100, 325, 325); // Draw Sun
// Using only one value generates a grayscale value.
c = color(65, 150, 0);
fill(c);

ellipse(300, 300, 150, 150); // Draw Mercury
  
  c=color (400,240,0);
  fill(c);
  arc(350, 175, 80, 80, 1100, PI + QUARTER_PI, PIE); //moon
  
  
quad(0, 0, 235, 15, 225, 190, 30, 240); //sun aesthetic
}
---------------------------------------------------------------------------------------------------------------------
//Lab 4

function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);
  
  if (mouseIsPressed === true  ){
  
  fill(235, 176, 66)
  
    ellipse(150, 150, 120, 120); // crust
  
  fill(235, 210, 101);
  
  ellipse (150, 150, 100, 100); //cheese
  
  
  var x = 125;
  while (x <= 175){
    
    fill(235, 89, 42);
     ellipse( x , 125,15,15);
    
    x = x+ 25;
  } //first row of toppings
  
  
  var x = 112;
  while (x <= 200){
    fill(235, 89, 42);
     ellipse( x , 150,15,15);
    
    x = x+ 25;
  } // second row of pizza toppings
  
    
   var x = 125;
  while (x <= 175){
    fill(235, 89, 42);
     ellipse( x , 175,15,15);
    
    x = x+ 25;
  } // third row of pizza toppings 
  ////////////////////////////////////////////
  } // end if and move to else if
  
   if (keyIsPressed === true) 
  {
    
    
  fill(235, 176, 66)
  
    ellipse(300, 150, 120, 120); // crust
  
  fill(235, 210, 101);
  
  ellipse (300, 150, 100, 100); //cheese
  
  
  var x = 275;
  while (x <= 325){
    
    fill(235, 89, 42);
     ellipse( x , 125,15,15);
    
    x = x+ 25;
  } //first row of toppings
  
  
  var x = 262;
  while (x <= 350){
    fill(235, 89, 42);
     ellipse( x , 150,15,15);
    
    x = x+ 25;
  } // second row of pizza toppings
  
    
   var x = 275;
  while (x <= 325){
    fill(235, 89, 42);
     ellipse( x , 175,15,15);
    
    x = x+ 25;
  } // third row of pizza toppings 
    
    
  }// end  if
  ////////////////////////////////////
  if ( mouseIsPressed && keyIsPressed === true) 
   {
    
    
  fill(235, 176, 66)
  
    ellipse(225, 275, 120, 120); // crust
  
  fill(235, 210, 101);
  
  ellipse (225, 275, 100, 100); //cheese
  
  
  var x = 200;
  while (x <= 250){
    
    fill(235, 89, 42);
     ellipse( x , 250,15,15);
    
    x = x+ 25;
  } //first row of toppings
  
  
  var x = 187;
  while (x <= 275){
    fill(235, 89, 42);
     ellipse( x , 275,15,15);
    
    x = x+ 25;
  } // second row of pizza toppings
  
    
   var x = 200;
  while (x <= 250){
    fill(235, 89, 42);
     ellipse( x , 300,15,15);
    
    x = x+ 25;
  } // third row of pizza toppings 
    
    
  }// end  if
  //////////////////////////////////////
 
   
    
    
  fill(235, 176, 66)
  
    ellipse(50 + mouseX, 275 + mouseY, 120, 120); // crust
  
  fill(235, 210, 101);
  
  ellipse (50 + mouseX, 275 + mouseY, 100, 100); //cheese
  
  
  var x = 25 ;
  while (x <= 75){
    
    fill(235, 89, 42);
     ellipse( x+ mouseX , 250 + mouseY,15,15);
    
    x = x+ 25;
  } //first row of toppings
  
  
  var x = 12;
  while (x <= 100){
    fill(235, 89, 42);
     ellipse( x+mouseX, 275 + mouseY,15,15);
    
    x = x+ 25;
  } // second row of pizza toppings
  
    
   var x = 25;
  while (x <= 75){
    fill(235, 89, 42);
     ellipse( x +mouseX , 300 + mouseY,15,15);
    
    x = x+ 25;
  } // third row of pizza toppings 
    
     
    
 
  
  
}
-----------------------------------------------------------------------------------------
//Lab 10


let duck;
let cam;
let movement = 0.01;

var panda;

function preload() {
  
  car = loadJSON("car.json");
  
}

function setup() {
  createCanvas(400, 400, WEBGL);
  
  
  fill(car.r, car.g, car.b);
  text(car.name, 10, 50);

   cam = createCamera();
  // set initial pan angle
  cam.pan(-0.4);
  
  
}

function draw() {
  background(60);

  
 
  
  
  
   // pan camera according to angle 'movement'
  cam.pan(movement);

  // every 100 frames, switch direction
  if (frameCount % 100 === 0) {
    movement *= -1;
  }
  
   ///// Sphere
  
  translate( 0, 0, 0);
    push();
   let dirX = 1;
  let dirY =  1;
    directionalLight(300, 0, 0, -dirX, -dirY, -1);
  rotateZ(frameCount * 0.01);
  rotateX(frameCount * 0.01);
  rotateY(frameCount * 0.01);
  sphere(30);
  pop();
  
    ////// Shape: Cube
  
  translate(-125, -125, -150);
  
  push();
  ambientLight(200);
  ambientMaterial(60, 180, 94);
  rotateZ(frameCount * 0.02);
  rotateX(frameCount * 0.02);
  rotateY(frameCount * 0.02);
  box(60, 60, 60);
  pop();

  
 ///// Shape: 8 sided 
  
   translate(0, 260, 100);
  
  push();
  ambientLight(200);
  normalMaterial();
  rotateZ(frameCount * 0.01);
  rotateX(frameCount * 0.01);
  rotateY(frameCount * 0.01);
  beginShape();
vertex(-10, 10);
vertex(0, 35);
vertex(10, 10);
vertex(35, 0);
vertex(10, -8);
vertex(0, -35);
vertex(-10, -8);
vertex(-35, 0);
endShape();
  pop();
  
}
