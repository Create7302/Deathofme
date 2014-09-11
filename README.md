Deathofme
=========

FB tab

<?php
if($_POST["submit"]) {
    $email_to="watershed@cityofdenton.com";
    $email_subject="Reverse Litter Contest Entry";
    $FirstName =$_POST["FirstName"];
    $LastName=$_POST["LastName"];
    $Email_Address=$_POST["Email_Address"];
    $ZIPcode=$_POST["ZIPcode"];
    $Category=$_POST["Category"];
    $ArtSummary=$_POST["ArtSummary"];
    $Answer=$_POST["Answer"];
    

?>


<!DOCTYPE html>
<html>
<body>
<form action= “processingscript.php” method= “post” enctype="multipart/form-data">
<p> <Strong> First Name</strong> </p>
<input name=“FirstName” size=“15” type=“text” />

<p> <Strong> Last Name</strong></p>
<input name=“LastName” size=“15” type=“text” />

<p> <Strong> Email Address</strong></p>
<input type = “email” name= “Email_Address” />
<input[type=email]:valid {background: green}/>
<input[type=email]:invalid {background: red}/>

<p> <Strong> Zip Code</strong></p>
<input type=“number” name=“ZIPcode” min= “5” max= “5” />
<input[type=number]:valid {background: green}/>
<input[type=number]:invalid {background: red}/>


<p> <Strong> Category</strong></p>
<select multiple= “multiple” name= “Category”>
<option> Elementary (K-5th grade) </option>
<option> Middle School (6th-8th grade) </option>
<option> High School (9th-12th grade) </option>
<option> College </option>
<option> Community</option>
<option> Senior Citizen (55+) </option>
</select>

<p> <Strong> Art Summary (Tell us about your art) </strong></p>
<TEXTAREA NAME= “ArtSummary” ROWS= 3 COLS= 30> </TEXTAREA>

<p> <Strong> I take the TEN on TUESDAY Pledge</strong></p>
<input type="checkbox" name="Answer" value="Yes">Yes, required for contest<br>
<input type="checkbox" name="Answer" value="No">No<br> 
<br>
<label for="file"><strong>Upload photo here:</strong></label>
<input type="file" name="file" id="file"><br>
<input type="submit" name="submit" value="Submit">

</form>

</body>
</html>
