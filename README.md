# new
var paintBrush = {
    x: 100,
    y: 300,
    img: getImage("avatars/mr-pants-with-hat")
};

var paintCanvas = function() {
    imageMode(CENTER);
    image(paintBrush.img, paintBrush.x, paintBrush.y);
};

mouseMoved = function() {
    paintBrush.x = mouseX;
    paintBrush.y = mouseY;
    paintCanvas();

};
paintCanvas();
