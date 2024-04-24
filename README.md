# Exercise2-image-processing-
img = zeros(500,500);
c_y = 250;
c_x = 250;
radius = 150;
for w = linspace(0 , 2*pi , 1000)
    y = round(c_y + radius * sin(w));
    x = round(c_x + radius * cos(w));
     if x >= 1 && x <= 500 && y >= 1 && y <= 500
         img(x,y)=255;
     end
end
imshow(img)
