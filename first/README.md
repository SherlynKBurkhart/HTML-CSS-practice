IF YOU ARE VIEWING THIS ON GITHUB, CHANGE THE VIEW TO "RAW".  IT WILL BE MUCH EASIER TO READ AND FOLLOW.

0. Change view to raw. (if you viewing on are on github)

This is an example of an instructional design that I created to assist an individual who asked me to teach them some basics of HTML and CSS.

This README.md file provides directions for a beginner learning how to work with HTML (HyperText Markup Language) and CSS (Cascading Style Sheets).

I work on a MacBook Pro and these directions are specific for Macs and some directions may be specific for my Mac due to individual settings on my computer.  Please email me at sherlynburkhart@gmail.com with any questions, comments, corrections, or clarifications.

This project creates boxes of different shapes and sizes with a place for text.


CREATE A "myProjects" FOLDER
1. Open "Finder".
2. Select "Desktop" on the left side of the window.
3. Select the settings caret at the top of the page ("settings" looks like a wheel, "caret" looks like a v).
4. Select "New Folder".
5. Type "myProjects" in place of "untitled folder" for the folder name. "myProjects" folder is where ALL of your projects are filed. 
6. Press "command S" to save.


CREATE A FOLDER FOR EACH INDIVIDUAL PROJECT
1. Open finder.
2. Select "Desktop".
3. Select "myProjects".
4. Select “Open”
5. Two finger click “myProjects” folder.
6. Select "New Folder”.
7. Type folder name. Suggestion - “myFirstProject”.
8. Select “enter/return” on keyboard.

INSTALL "SUBLIME TEXT"
1. Google "Sublime Text" and download the latest version on your computer.
2. Open "Sublime Text".
3. Drag and drop "myProjects" folder into sublime text
	

CREATE AN HTML (HyperText Markup Language) FILE - THIS IS DONE IN SUBLIME TEXT
1. Two finger click (it is a Mac thing) “myFirstProject” folder.
2. Select “New File”.
3. Type "index.html". This names the file.
4. Press "command S” to save. 
5. Confirm that the file is being saved in "myFirstProjects".
6. Select “Save”. (A pop-up to purchase may occur - you may press cancel.)
7. Delete “index.html” on line one.
8. Type “<!DOCTYPE html”.
9. Press “tab” key. Walla!! The below opening and closing tags appear. This is the basic HTML (HyperText Markup Language) file structure.

<!DOCTYPE <!DOCTYPE html>   (This first line may look like "<!DOCTYPE <html>")
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>


WRITE CODE INTO THE "index.html" FILE
IMPORTANT NOTE!  Typing accuracy is essential in code. Make sure the spaces, or lack thereof, between the words are correct. They could be the difference in your code working correctly or not. 
1. Between opening and closing title tags "<title></title>" type: 
 	practicing HTML

2. Press return.
3. Type or copy and paste:
	<!-- links -->
	<link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.css">
	<link type="text/css" rel="stylesheet" href="styles.css"> 

4. On the line directly above the closing body tag, "</body>" type:
	<!-- sources -->
	<script src="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.js"></script>	

5. Right after the opening body tag <body>, on the next line type:
	<!-- first row - red box, blue box, grey box -->
	<div layout="row">
		<div flex="30" 
			class="row1 boxRed">
		</div>
		<div flex="30" 
			offset="5" 
			class="row1 boxBlue">
		</div>
		<div flex="30" 
			offset="5" 
			class="row1 boxGrey">
		</div>
	</div>

6. Press "command S" to save.	


CREATE A CSS (Cascading Style Sheets) FILE
1. Two finger click “myFirstProject” folder.
2. Select “New File”.
3. Type "styles.css".
4. Press "command S” to save. 
5. Confirm that the file is being saved in "myFirstProjects".
6. Select “Save”.  (A pop-up to purchase may occur - you may press cancel.)
7. Delete “styles.css” on line one.


WRITE CODE INTO THE "styles.css" FILE
1. Beginning at the top of the page type:

html, body { 
  margin: 15px 10px 15px 10px;
}

/*colors*/
.boxRed {
  background: #D50000;
}

.boxBlue {  
  background: #2196F3;
}

.boxGrey {
  background: #424242;
}

/*first row*/
.row1 {
  height: 200px;
}

2. Save (command S).


VIEW FILE IN BROWSER - ONLY OPENS IN CHROME
1. Install "Chrome" browser if it is not installed on your computer.
	A. Google "chrome".
	B. Install latest version.
1. In Sublime Text move cursor over index.html file text window space.
2. Two finger click.
3. Select "Open in Browser" in grey popup box.
4. Files are opened in Chrome.
5. You should see three boxes with the colors red, blue, and grey.


WRITE MORE CODE INTO THE "index.html" FILE
0. After the code you already typed into "index.html" file under "<body>", type:

	<!-- second - text area -->
	<div layout="column" class="textAll">
		<p>This area is for the first paragraph.
		</p>
		<p>This area is for a second paragraph.
		</p>
	</div>

	<!-- third row - red box, blue box -->
	<div layout="row">
			<div flex="33"
				class="row3 boxRed">
			</div>
			<div flex="66"
				class="row3 boxBlue">
			</div>
		</div>

		<!-- fourth row - blue box, grey box inside red box -->
	<div layout="row">
		<div flex="66"
			class="row4 boxBlue">
		</div>
		<div flex="33"
			class="row4 boxRed">
				<div class="row4 boxGrey"></div>
			</div>	
	</div>

1.Save.


WRITE MORE CODE INTO THE "styles.css" FILE
0. After the code you already typed into the "styles.css" file, type:

/*second - text area*/
.textAll {
  height: 450px;
  font-family: sans-serif;
  margin-right: 50px;
  font-size: 25px;
}

/*third row*/
.row3 {
  height: 500px;
}

/*fourth row*/
.row4 {
  margin: 30px 0 30px 0;
  height: 200px;
}

.row4.boxGrey {
  margin: 0 45px 0 45px;
  width: 325px;
}

1. Save.


THIS IS WHAT THE COMPLETED "index.html" FILE LOOKS LIKE

<html>
	<head>
		<title>practicing HTML
		</title>

		<!-- links -->
	    <link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.css">
		<link type="text/css" rel="stylesheet" href="styles.css">
	</head>

	<body>

		<!-- first row - red box, blue box, grey box -->
		<div layout="row">
			<div flex="30" 
				class="row1 boxRed">
			</div>
			<div flex="30" 
				offset="5" 
				class="row1 boxBlue">
			</div>
			<div flex="30" 
				offset="5" 
				class="row1 boxGrey">
			</div>
		</div>

		<!-- second - text area -->
		<div layout="column" class="textAll">
			<p>This area is for the first paragraph.
			</p>
			<p>This area is for a second paragraph.
		</div>

		<!-- third row - red box, blue box -->
		<div layout="row">
  			<div flex="33"
  				class="row3 boxRed">
  			</div>
  			<div flex="66"
  				class="row3 boxBlue">
  			</div>
  		</div>

  		<!-- fourth row - blue box, grey box inside red box -->
		<div layout = "row">
			<div flex="66"
				class="row4 boxBlue">
			</div>
			<div flex="33"
				class="row4 boxRed">
  				<div class="row4 boxGrey"></div>
  			</div>	
		</div>

		<!-- sources -->
		<script src="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.js">
		</script>

	</body>
</html>


THIS IS WHAT THE COMPLETED "styles.css" FILE LOOKS LIKE

html, body { 
  margin: 15px 10px 15px 10px;
}

/*colors*/
.boxRed {
  background: #D50000;
}

.boxBlue {  
  background: #2196F3;
}

.boxGrey {
  background: #424242;
}

/*first row*/
.row1 {
  height: 200px;
}

/*second - text area*/
.textAll {
  height: 450px;
  font-family: sans-serif;
  margin-right: 50px;
  font-size: 25px;
}

/*third row*/
.row3 {
  height: 500px;
}

/*fourth row*/
.row4 {
  margin: 30px 0 30px 0;
  height: 200px;
}

.row4.boxGrey {
  margin: 0 45px 0 45px;
  width: 325px;
}


TIME TO PLAY - FURTHER UNDERSTANDING HTML
(I AM USING HTML AND ANGULAR MATERIAL DESIGN HERE)
0. Find the "flex" property inside the <body>. 
1. Change the "flex" numbers to 5, 10, and 15.
2. Press "command S".
3. Repeat the exploration!


TIME TO PLAY - FURTHER UNDERSTANDING CSS (Cascading Style Sheets) COLORS
0. In your Chrome browser go to website https://www.google.com/design/spec/style/color.html#
1. Scroll down the page to see all the colors!
2. Pick any color identifier (it looks like #000000, and has numbers and letters).
3. Open the "styles.css" file.
4. Replace the color identifier of "background: #D50000" in the "styles.css" file with the color of your choice.
5. Press "command S".
6. Go to your Chrome browser and press "command R" to refresh the browser. The color has changed!
7. Repeat the fun!


TIME TO PLAY - FURTHER UNDERSTANDING CSS PROPERTIES
0. Adjust the margin, height, and width numbers.
1. Save.
2. Refresh Chrome browser.
3. Repeat the fun!


FAQ's
HOW DOES THE index.html FILE KNOW TO USE THE styles.css FILE?
<link type="text/css" rel="stylesheet" href="styles.css">
"href" means hyperlink reference. The reference is the "styles.css" file.

WHAT IS A GOOD LINK TO LEARN MORE ABOUT HTML?
http://www.w3schools.com/html/html_intro.asp

HOW DOES THE HTML FILE AND CSS FILE TALK TO EACH OTHER? In the <body> of "index.html", each <div> (short for a division of space) has a "class" attribute. Each "class" attribute is equal to a camelCase name chosen by the programmer. That name is then used in the css file to give characteristics to the element.

WHAT IS A GOOD LINK TO LEARN MORE ABOUT CSS?
https://developer.mozilla.org/en-US/docs/Web/CSS/Reference

WHAT IS THE DIFFERENCE BETWEEN AN 0PENING AND CLOSING TAG?
An opening tag does not have a backslash "/". A closing tag has the "/", . ie. opening tag <body>, closing tag </body>.


PLEASE EMAIL ME AT SherlynBurkhart@gmail.com WITH ANY OTHER QUESTIONS YOU MAY HAVE!
