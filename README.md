# ooh-lala
2018 HTML Term III Page Repository Suhyun Yun
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>Untitled Document</title>
<link href="Forms.css" rel="stylesheet" />
</head>

<body>
	<form name="CindyQuiz">
    	<fieldset>
        <legend>Cindy's Quiz</legend>
        <div>
        	<fieldset>
            <legend>Question #1</legend>
        	<p>What is the name of the artist that sang "Perfect?"</p>
            <input type="radio" name="onechoice" value="Ted"/> Ted
            <br />
            <input type="radio" name="onechoice" value="Ed"/> Ed
            <br />
            <input type="radio" name="onechoice" value="Zedd"/> Zedd
            <br />
            <input type="radio" name="onechoice" value="Ad"/>Ad
            </fieldset>
        </div>
        <div>
        	<fieldset>
            <legend>Question #2</legend>
        	<p>Which artist has sung with Ed Sheeran?</p>
            <input type="checkbox" name="multiple1" value="Psy" /> Psy
            <br />
            <input type="checkbox" name="multiple2" value= "Beyonce" />  Beyonce
            <br />
            <input type="checkbox" name="multiple3" value="Taylor Swift" /> Taylor Swift
            <br />
            <input type="checkbox" name="multiple4" value= "Nicki Minaj" /> Nicki Minaj
            <br />
            <input type="checkbox" name="multiple5" value="John Mayer"/> John Mayer
            <br />
            
            </fieldset>
        </div>
        <div>
        <fieldset>
            <legend>Question #3</legend>
        	<p>What color is Ed Sheeran's 'Plus' album? </p>
            <select>
            	<option value="Red"> Red </option>
                <option value="Orange"> Orange </option>
                <option value="Green">Green </option>
                <option value="Blue">Blue </option>
            </select>
        </fieldset>
        </div>
        <div>
        <fieldset>
            <legend>Question #4</legend>
        	<p>What is Ed Sheeran's middle name? </p>
            <input name="q4" type="text" placeholder="Answer here" />
        </fieldset>
        </div>
        <div>
        <fieldset>
            <legend>Question #5</legend>
        	<p> Fill in the blanks: "Taylor Swift's 5th studio album is called<input name="q5"type="color"/>"</p>
            
        </fieldset> 
        </div>
        <div>
        <fieldset>
            <legend>Question #6</legend>
        	<p> Which song is not Ed Sheeran's? </p>
            <input type="button" value="Firefly" />
            <input type="button" value="Kiss me" />
            <input type="button" value="Chasing Cars" />
            <input type="button" value="Cold Coffee" />
        </fieldset>
        </div>
        <div>
        	<p>Thanks for playing!</p>
        	<input type="submit" onclick="answerChecker()"/>
        </div>
        </fieldset>
    </form>
     <script>
	function answerChecker() {
		//checks which radio button is selected
		if(document.CindyQuiz.onechoice.value==="Ed") {
			alert("Question 1 is correct!");
		} else {
			alert("Question 1 WRONG!");
		}
		
		//checks which checkboxes are clicked
		if(document.CindyQuiz.multiple2.checked===true && document.CindyQuiz.multiple3.checked===true && document.CindyQuiz.multiple5.checked===true && document.CindyQuiz.multiple1.checked===false && document.CindyQuiz.multiple4.checked===false) {
			alert("Question 2: He/She did sing with Ed!");
		} else {
			alert("Question 2: Nope. Not this person.");
		}
		
		//checks which option is chosen on select menu
		if(document.CindyQuiz.q3.value==="Orange") {
			alert("Question 3: Correct!");
		} else {
			alert("Question 3: No, that's not it.");
		}
		
	}
		//checks what is typed into textbox on question 4
		if(document.CindyQuiz.q4.value==="Christopher") {
			alert("Question 4 is correct!");
		} else {
			alert("Nope on Question 4");
		}
		
		//checks which color was selected on the color picker
		if(document.CindyQuiz.q5.value==="#ff0000") {
			alert("Question 5: Red! Correct!");
		} else {
			alert("Question 5: No, that's not it.");
		}
	</script>
</body>
</html>
