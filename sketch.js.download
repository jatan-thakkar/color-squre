var canvas;
var music;
var rectangle1,rectangle2,rectangle3,rectangle4
var squre
var edges
function preload(){
    music = loadSound("music.mp3");
    
}


function setup(){
    canvas = createCanvas(800,600);

    //create 4 different surfaces
rectangle1 = createSprite(0,580,360,30)
rectangle1.shapecolor = rgb(0,0,255)

rectangle2 = createSprite(295,580,200,30)
rectangle2.shapecolor = rgb(255,128,0)

rectangle3 = createSprite(515,580,200,30)
rectangle3.shapecolor = rgb(153,0,76)

rectangle4 = createSprite(740,580,220,30)
rectangle4.shapecolor = rgb(0,100,0)

squre = createSprite(random(20,750),100,40,40)
squre.shapecolor = rgb(255,255,255)
squre.velocityX = 4;
squre.velocityY = 9;
    //create box sprite and give velocity
    


}

function draw() {
    background(rgb(169,169,169));
    edges=createEdgeSprites();
    squre.bounceOff(edges);

    if(rectangle1.isTouching(squre) && squre.bounceOff(rectangle1)){
       squre.shapeColor = rgb(0,0,255);
       music.play();
    }
   if(rectangle2.isTouching(squre)){
    squre.shapeColor = rgb(255,128,0)
     squre.velocityX = 0;
     squre.velocityY = 0;
    music.stop();
   }

   if(rectangle3.isTouching(squre) && squre.bounceOff(rectangle3)){
       squre.shapecolor = rgb(153,0,76);
   }

  if(rectangle4.isTouching(squre) && squre.bounceOff(rectangle4)){
      squre.shapeColor = rgb(0,100,0);
  }
drawSprites();
    //add condition to check if box touching surface and make it box
}
