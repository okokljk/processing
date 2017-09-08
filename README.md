# processing

코드






 int x = 300;
int y = 200;
int dirX= 20;
int dirY= 20;



void setup () {
  size(1200, 600);
   background(x,y,150);
}

void draw() {
  
 
  fill(mouseX,mouseY ,1);
  ellipse(x, y, 50, 50);
  
  if( x>width ||x<0) {
    dirX*= -1;
  }
  if( y>height ||y<0) {
    dirY*= -1;
  }
  
  
  x = x+dirX;
  y = y+dirY;
  
 
 
  println(x,y);
  
  
  
  
 랜덤코드







void setup() {
  size(600,600);
  background(255);
  
}

void draw () {
  r = random(255);
  g = random(255);
  b = random(255);
  a = random(255);
  diam = random(20);  //도형의 크기
  x = random(width);
  y = random(height);
  
  noStroke();
  fill(r,g,b,a);
  rect(x,y,diam,diam);
}

 

    

 
 주그캐릭터





float zoogX;
float zoogY;

float eyeR;
float eyeG;
float eyeB;
int x= 20;
void setup(){
  size(1200,960);
  zoogX= width/2;
  zoogY= height + 100;
}
void draw() {
  background(150,20,53);
  
  ellipseMode(CENTER);
  rectMode(CENTER);
  
  stroke(0);
  fill(150);
  rect(zoogX,zoogY,20,100);
  
  stroke(0);
  fill(255);
  ellipse(zoogX,zoogY-30,60,60);
  
  eyeR = random(255);
  eyeG = random(255);
  eyeB = random(255);
  fill(eyeR, eyeG, eyeB);
  ellipse(zoogX-19,zoogY-30,16,32);
  ellipse(zoogX+19,zoogY-30,16,32);
  
  stroke(150);
  line(zoogX-10, zoogY+50, zoogX-10, height);
  line(zoogX+10, zoogY+50, zoogX+10, height);

  zoogY=zoogY-1;
    
   
  
 
   
  
  
  
  
  
}
 
 
 
 
 
 
 
   주그 마우스로 제어하기
   
   
   
   
   
   
   
   void setup(){
  size(1200,960);
 
}
void draw() {
  background(150,20,53);
  
  ellipseMode(CENTER);
  rectMode(CENTER);
  
  translate(mouseX,mouseY);
  
  stroke(0);
  fill(214);
  rect(0,0,20,100);
  
  stroke(0);
  fill(255);
  ellipse(0,-30,60,60);
}
