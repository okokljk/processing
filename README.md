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
  

 

    

 
}
