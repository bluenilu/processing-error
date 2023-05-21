int cellSize = 80;
int[][] cells;
int X, Y;

color yellow;
float thresholdline = 40;

void setup () {
  size(640, 480);
  yellow = color(#FAFF00);

  cells = new int[width/cellSize][height/cellSize];
  for (int i=0; i<width/cellSize; i++) {
    for (int j=0; j<height/cellSize; j++) {
      rect (i*cellSize, j*cellSize, cellSize, cellSize);
    }
  }

  float px1 = random(0, 640);
  float py1 = 0;
  float px2 = random(0, 480);
  float py2 = random(120, 240);
  float px3 = random(0, 640);
  float py3 = random(240, 360);
  float px4 = random(0, 640);
  float py4 = 480;
  strokeWeight (5);
  stroke (#FAFF00);

  line (px1, py1, px2, py2);
  line (px2, py2, px3, py3);
  line (px3, py3, px4, py4);
}

void draw() {
  loadPixels(); // load the pixel array

  for (int x = 0; x < width; x ++ ) {
    for (int y = 0; y < height; y ++ ) {


      if (get(x, y) == yellow) { // check if the cell has a yellow pixel
        fill(0); 
        rect(x, y, cellSize, cellSize); // fill the cell with a black rectangle
      }
    }
  }
}
