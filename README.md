<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script type="text/javascript" src="scripts/jquery-3.4.1.min.js"></script>
    
    <!-- validation script -->
<script>
        
</script>


</head>
<body style="background-color: antiquewhite;">
    
<center><h2 style="color: brown;"><u>Student Registration Form</u></h2></center>
<form action="" method="POST" name="regform" onsubmit="return validation()">
    <fieldset style="border-color:darkcyan;">
        <legend>Personal</legend>
        <table>
            <tr>
                <td>Name :</td>
                <td><input type="text" class="text" name="name" placeholder="Name" ></td>
            </tr>
            <tr>
                <td>Father's Name :</td>
                <td><input type="text" class="text" name="fname" placeholder="Father's Name" ></td>
            </tr>
            <tr>
                <td>Mother's Name :</td>
                <td><input type="text" class="text" name="mname" placeholder="Mother's Name" ></td>
            </tr>
            <tr>
                <td>Date of Birth :</td>
                <td><input type="date" class="text" name="date" placeholder="Date of Birth" ></td>
            </tr>
            <tr>
                <td>Address (Permanent address) :</td>
                <td><textarea name="addressP" id="" cols="30" rows="5" placeholder="Permanent Address"></textarea></td>
            </tr>
            <tr>
                <td>Address (Temporary address) :</td>
                <td><textarea name="addressC" id="" cols="30" rows="5" placeholder="Current Address" ></textarea></td>
            </tr>
            <tr>
                <td>Gender :</td>
                <td>Male :<input type="radio" name="gender" class="radio">Female<input type="radio" name="gender" class="radio"></td>
            </tr>
            <tr>
                <td>Phone Number (Parent) :</td>
                <td><input type="text" class="text" name="fnumber" placeholder="Fathers Number" ></td>
            </tr>
            <tr>
                <td>Phone Number (Student) :</td>
                <td><input type="text" class="text" name="pnumber" placeholder="Personal Number" ></td>
            </tr>
            <tr>
                <td>Email ID :</td>
                <td><input type="text" name="email" placeholder="Email" ></td>
            </tr>
            <tr>
                <td>Applying for Course :</td>
                <td>
                    <select id="course" name="course">
                        <option value="diploma">Diploma</option>
                        <option value="degree">Degree</option>
                    </select>
                </td>
            </tr>
            <tr>
                <td>Choose Department :</td>
                <td>
                   
                  <input type="checkbox"  name="cse">CSE&nbsp;
                   <input type="checkbox"  name="civil">CIVIL&nbsp;
                   <input type="checkbox"  name="ece">ECE&nbsp;
                   <span id="Dip">
                        <input type="checkbox"  name="elec">ELEC&nbsp;
                        <input type="checkbox"  name="mech">MECH&nbsp;
                        <input type="checkbox"  name="it">IT&nbsp;
                        <input type="checkbox"  name="dhmct">DHMCT&nbsp;
                        <input type="checkbox"  name="pdme">PDME&nbsp;
                   </span>
                </td>
            </tr>
        </table>
    </fieldset>
    <br>
    <fieldset style="border-color:darkcyan;">
        <legend>Qualification :</legend>
        <span id="ten">
        <table>
            
                <tr>
                    <td>10<sup>th</sup> Board :</td></td>
                    <td><input type="text" name="tenb" id="10b" placeholder="Board" ></td>
                </tr>
                <tr>
                    <td>10<sup>th</sup> percentage :</td>
                    <td><input type="text" name="tenp" id="10b" placeholder="Percentage" ></td>
                </tr>
                <tr>
                    <td>Year of passing :</td>
                    <td><input type="text" name="teny" id="tnyear" placeholder="Year of passing" ></td>
                </tr>
            
            </table>
        </span>
        <span id="twel">
            <table>
            
                <tr>
                    <td>12<sup>th</sup> Board :</td>
                    <td><input type="text" name="twelb" id="12b" placeholder="Board"></td>
                </tr>
                <tr>
                    <td>12<sup>th</sup> percentage :</td>
                    <td><input type="text" name="twely" id="12b" placeholder="Percentage" ></td>
                </tr>
                <tr>
                    <td>Year of passing :</td>
                    <td><input type="text" name="twelp" id="twyear" placeholder="Year of passing" ></td>
                </tr>
                </table>
            </span>
            <table>


            <tr>
                <td>Any other Qualification</td>
                <td>
                    <select name="" id="qualification">
                        <option value="text1">Diploma in Computer Application</option>
                        <option value="text2">Tally with GST</option>
                        <option value="text2">Others</option>
                        <option value="text2">Don't Have</option>
                    </select>
                </td>
                <td><input type="file" name="" id="file" ></td>
            </tr>
            <tr>
                <td>Preferences</td>
                <td>
                    <select name="1p" id="1p">
                        <option value="">1st Preference</option>
                        <option value="BCSE" id="btech" class="btech">Btech. CSE</option>
                        <option value="BCIVIL" id="btech" class="btech">Btech. CIVIL</option>
                        <option value="BECE" id="btech" class="btech">Btech. ECE</option>
                        <option value="DCE" id="dip" class="dip">DCE</option>
                        <option value="DECE" id="dip" class="dip">Dip. ECE</option>
                        <option value="DCVIL" id="dip" class="dip">Dip. Civil</option>
                        <option value="DIT" id="dip" class="dip">Dip. IT</option>
                        <option value="DMECH" id="dip" class="dip">Dip. MECH</option>
                        <option value="DELEC" id="dip" class="dip">Dip. ELEC</option>
                    </select>
                </td>
                <td>
                    <select name="2p" id="2p">
                        <option value="">2nd Preference</option>
                        <option value="BCSE" id="btech" class="btech">Btech. CSE</option>
                        <option value="BCIVIL" id="btech" class="btech">Btech. CIVIL</option>
                        <option value="BECE" id="btech" class="btech">Btech. ECE</option>
                        <option value="DCE" id="dip" class="dip">DCE</option>
                        <option value="DECE" id="dip" class="dip">Dip. ECE</option>
                        <option value="DCVIL" id="dip" class="dip">Dip. Civil</option>
                        <option value="DIT" id="dip" class="dip">Dip. IT</option>
                        <option value="DMECH" id="dip" class="dip">Dip. MECH</option>
                        <option value="DELEC" id="dip" class="dip">Dip. ELEC</option>
                    </select>
                </td>
                <td>
                    <select name="3p" id="3p">
                        <option value="">3rd Preference</option>
                        <option value="BCSE" id="btech" class="btech">Btech. CSE</option>
                        <option value="BCIVIL" id="btech" class="btech">Btech. CIVIL</option>
                        <option value="BECE" id="btech" class="btech">Btech. ECE</option>
                        <option value="DCE" id="dip" class="dip">DCE</option>
                        <option value="DECE" id="dip" class="dip">Dip. ECE</option>
                        <option value="DCVIL" id="dip" class="dip">Dip. Civil</option>
                        <option value="DIT" id="dip" class="dip">Dip. IT</option>
                        <option value="DMECH" id="dip" class="dip">Dip. MECH</option>
                        <option value="DELEC" id="dip" class="dip">Dip. ELEC</option>
                    </select>
                </td>
            </tr>
           
        </table>
    </fieldset>
    <br>
    <center>
    <input type="submit" id="submit" value="Submit">
    <input type="reset" value="Reset">
    </center>
</form>
<script type="text/javascript" src="Dept.js"></script>
<script type="text/javascript" src="Validation.js"></script>
</body>
</html>
