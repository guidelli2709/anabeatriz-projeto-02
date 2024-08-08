function setup() {

createCanvas (400, 400); }

function draw() {

background(220); }let cor;

let circulox;

let circuloy;

function setup() {

createCanvas(400, 400);

background(color (100, 0, 0));

cor color(random (0, 255), random (0, 255), random(0, 255));

circulox = [0, 0, 0];

circuloy = [random(height), random (height), random(height)];

}

function draw() {

fill(cor);

for (let contador in circulox) {

circle(circulox [contador], circuloy [contador], 50);

circulox[contador] += random(0, 3);

circuloy [contador] += random(-3, 3);

if (circulox [contador] >= width) {

circulox[contador] = 0;

circuloy [contador] = random(height);

}

}

if (mouseIsPressed) {

cor color(random(0, 255), random (0, 255), random(0, 255), random (0, 100));

}

}
