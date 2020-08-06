# googleColor

This piece of program simply changes that color of the "Google" logo on the google home page

To execute this script you need to open google homne page;
step 1) Right click anywhere on the google homne page and click on "inspect" or you can use shortcut Ctrl+Shift+I
step 2) Now at he top of inspect section you migh see few tabs namely "Elements", "Console", Sources" etc... You need to click on Sources tab
step 3) On the very left you'll see a Snippets section click on it and below that click on "New Snippet" to creat new snippet
step 4) Create a new snippet name it "index.js" and past the given script into it (You can copy the script from below)


-----------------------------------------------------------------------COPY FROM HERE--------------------------------------------------------------------------------------

var keyStrokes = document.addEventListener("keydown", function(event){
  console.log(event.key);
  googleColor(event.key);
})

var google = document.querySelector(".show-logo")


function googleColor (keyStrokes){
  switch(keyStrokes) {
  case "a":
    google.style = "background-color: red;"
    break;
  case "s":
    google.style = "background-color: blue;"
    break;
  case "d":
    google.style = "background-color: green;"
    break;
  case "f":
    google.style = "background-color: yellow;"
    break;

  case "j":
    google.style = "background-color: orange;"
    break;
  case "k":
    google.style = "background-color: purple;"
    break;
  case "l":
    google.style = "background-color: brown;"
    break;
  case "s;":
    google.style = "background-color: black;"
    break;





  default:
    google.style = "background-color: white;"
}
}

------------------------------------------------------------------------------------------------------------------------------------------------------------------------
