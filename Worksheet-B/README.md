
Fallout 4 mini game procedure
	Create multiple arrays of 4 letter words 
	"Array" = Array selected at random from multiple arrays           
	"SecretWord" = Word selected at random from "Array" 
	"AttemptsRemaining" = 4
	"Likness" = 0

	Print 'Welcome to ROBCO Industries (TM) Termlink'
	Print 'Password Required'

	WHILE "Likeness" < 4 and "AttemptsRemaing" > 0 DO	    	 # Ends loop when player guesses correctly, or after four incorrect guesses
		"Likeness" = 0						                     # Resets the likness back to 0 after an incorrect guess
		Print 'Attempts Remaining: "AttemptsRemaining" '         # Displays 'Attempts Remaining: x' where x is No. of attempts remaining
		Print "Array"
		"WordGuessed" = The word the player enters
		If first letter of "WordGuessed" is the same as first letter of "SecretWord" Do
			Increase "Likeness" by 1
		If second letter of "WordGuessed" is the same as second letter of "SecretWord" Do
			Increase "Likeness" by 1
		If third letter of "WordGuessed" is the same as third letter of "SecretWord" Do
			Increase "Likeness" by 1
		If fourth letter of "WordGuessed" is the same as fourth letter of "SecretWord" Do
			Increase "Likeness" by 1

		Print 'Likness = "Likeness" '
		Decrease "AttemptsRemaining" by 1
	END WHILE
	
	If "AttemptsRemaining" > 0 Do
		print "Password Accepted"
	Else Print "You failed, Nice Try"
END
	
![alt tag](https://raw.githubusercontent.com/JonnyMarx98/comp110-worksheets/master/Worksheet-B/flowchart%20fallout%204.PNG)
