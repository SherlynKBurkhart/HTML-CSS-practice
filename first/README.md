This is an example of an instructional design that I created to assist an individual who asked me to teach them some basics of HTML and CSS.

This README.md file provides directions for a beginner learning how to work with HTML (HyperText Markup Language) and CSS (Cascading Style Sheets).

I work on a MacBook Pro and these directions are specific for Macs and some directions may be specific for my Mac due to individual settings on my computer.  Please email me at sherlynburkhart@gmail.com with any questions, comments, corrections, or clarifications.

The objective of this particular project is to make a page that looks as close to "first.png" as possible.


CREATE A "myProjects" FOLDER
0. Open "Finder".
1. Select "Desktop" on the left side of the window.
2. Select the settings caret at the top of the page ("settings" looks like a wheel, "caret" looks like a v).
3. Select "New Folder".
4. Type "myProjects" in place of "untitled folder" for the folder name. "myProjects" folder is where ALL of your projects are filed. 
5. Press "command S" to save.


CREATE A FOLDER FOR EACH INDIVIDUAL PROJECT
0. Google "Sublime Text" and download the latest version on your computer.
1. Open "Sublime Text"and make a new “myProjects” folder. 
	A. Your computer's file system opens.
	B. Select "Desktop".
	C. Select "myProjects".
	D. Select “Open”
	E. Two finger click “myProjects” folder.
	F. Select "New Folder”.
	G. Type folder name. Suggestion - “myFirstProject”.
	H. Select “enter/return” on keyboard.


CREATE AN HTML (HyperText Markup Language) FILE
0. Two finger click “myFirstProject” folder.
1. Select “New File”.
2. Type "index.html".
3. Press "command S” to save. 
4. Confirm that the file is being saved in "myFirstProjects".
5. Select “Save”. (A pop-up to purchase may occur - you may press cancel.)
6. Delete “index.html” on line one.
7. Type “<!DOCTYPE h”.
8. Press “Return” key.
9. Tab. Walla!! The below opening and closing tags appear. This is the basic HTML (HyperText Markup Language) file structure.

<!DOCTYPE <!DOCTYPE html>
<html>
<head>
	<title></title>
</head>
<body>

</body>
</html>

10. Delete "<!DOCTYPE ".


WRITE CODE INTO THE "index.html" FILE
IMPORTANT NOTE!  Typing accuracy is essential in code. Make sure the spaces, or lack thereof, between the words are correct. They could be the difference in your code working correctly or not. 
0. Between opening and closing title tags "<title></title>" type: 
 	practicing HTML

1. On the next line and in line with the opening title tag, "<title>", type: 
	<!-- links -->
	<link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.css">
	<link type="text/css" rel="stylesheet" href="styles.css"> 

2. On the line directly above the closing body tag, "</body>" type:
	<!-- sources -->
	<script src="https://ajax.googleapis.com/ajax/libs/angular_material/0.9.4/angular-material.min.js"></script>	

3. After the opening body tag <body>, on the next line, and in line with, type:
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

4. Press "command S" to save.	


CREATE A CSS (Cascading Style Sheets) FILE
0. Two finger click “myFirstProject” folder.
1. Select “New File”.
2. Type "styles.css".
3. Press "command S” to save. 
4. Confirm that the file is being saved in "myFirstProjects".
5. Select “Save”.  (A pop-up to purchase may occur - you may press cancel.)
6. Delete “styles.css” on line one.


WRITE CODE INTO THE "styles.css" FILE
0. Beginning at the top of the page type:

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

1. Save (command S).


VIEW FILE IN BROWSER - ONLY OPENS IN CHROME
0. Install "Chrome" browser if it is not installed on your computer.
	A. Google "chrome".
	B. Install latest version.
1. In Sublime Text move cursor over index.html file.
2. Two finger click.
3. Select "Open in Browser" in grey popup box.
4. Files are opened in Chrome.


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


COMPLETED "index.html" FILE

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


COMPLETED "styles.css" FILE

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
0. In your Chrome browser go to websitehttps://www.google.com/design/spec/style/color.html#
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


PLEASE EMAIL ME AT SherlynBurkhart@gmail.com WITH ANY OTHER QUESTIONS YOU MAY HAVE!