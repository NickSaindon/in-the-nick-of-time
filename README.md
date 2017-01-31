How to Create and Animation using a Sprite Image and CSS3 Key-frame

    Create a wrapper (window to display the image) to nest the image inside.
    Create another div for the background image inside the wrapper.
    Add the background image within the url and set the width and height to each individual frame.
    Set the background-size to the full width and height of the entire sprite image.
    Create an animation by adding a name, duration, number of steps (how many frames there are), and set it to infinite to loop the animation.
    Be sure to set all your margins to align the sprite to the center of the window.
    Create a key-frame and set the beginning to 0px and the from to 4400px (full width of the sprite).

`
.walk-wrapper {
width: 100%;
margin: 90px auto;
text-align: center;
}

#walking-sprit {
background-image:url(your-sprit-image.jpg);
background-size: 4400px 300px;
width: 400px;
height: 300px;
margin: 0 auto;
animation: walking-sprit 1s steps(11) infinite;
}

@keyframes walking-sprit {
to { background-position: 0px; }
from { background-position: 4400px; }
}
`
