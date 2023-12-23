<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Obour Students Management</title>
        <!-- restore fonts online link-->
        <link rel="preconnect" href="https://fonts.googleapis.com" />
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
        <link href="https://fonts.googleapis.com/css2?family=Libre+Franklin&display=swap" rel="stylesheet" />
        <link rel="preconnect" href="https://fonts.googleapis.com" />
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
        <link href="https://fonts.googleapis.com/css2?family=Beau+Rivage&display=swap" rel="stylesheet" />

        <script>
            //show alert to Delete All Students
            function showWarning() 
            {
            // Display a confirmation dialog
            var isConfirmed = confirm("Are you sure you want to delete all students?");
            if(isConfirmed) 
            {
                alert("All students have been successfully deleted");
            } 
            else 
            {
                alert("Action canceled!");
            }
            }
            //Generate Random Number to ID
            function generateRandomNumber() 
            {
            // Generate a random number between 1000 and 9999
            var randomNum = Math.floor(Math.random() * (9999 - 1000 + 1)) + 1000;
            // Fill the input field with the generated random number
            document.getElementById("ID").value = randomNum;
            }

        </script>

        <style>
            /*restore fonts As a file from the device*/
            @font-face
            {
                font-family: 'RubikLines-Regular';
                src:url(RubikLines-Regular.ttf); 
            }

            @font-face
            {
                font-family: 'BeauRivage';
                src:url(BeauRivage-Regular.ttf); 
            }

            @font-face
            {
                font-family:'RubikDoodleShadow';
                src:url(RubikDoodleShadow.ttf); 
            }

            @font-face
            {
                font-family:'LibreBaskerville';
                src:url(LibreBaskerville-Italic.ttf); 
            }

            body 
            {
                font-family: "Libre Franklin",sans-serif;
                margin: 0px;
            }

            header
            {
                padding-top:18%;
                padding-bottom: 0.1%;
                background-image:url("BG_header.JPEG");
                background-repeat: no-repeat;
                background-attachment:scroll;
                background-size: 100% 100%;   
            }       

            header a
            {
                position: relative;
                bottom: 260px;
                left: 10px;
                cursor: pointer;
            }

            header .h1 
            {
                /* cornflowerblue crimson */
                color: darkslateblue ;
                font-family: "Beau Rivage", cursive;
                font-size: 66px;
                position: relative;
                bottom: 510px;
                left: 200px;
            }

            nav
            {
                position: fixed;
                font-family:RubikLines-Regular,courier;
                font-size: x-large;    
                bottom: 55px;   
            }

            .OHIico
            {
                position:fixed;
                width: 90px;
                height: 80px;
                bottom: 5px;
                left:540px; 
            }

            nav .Sup
            {
                background-color: red;
                position:absolute;
                left: 638px;
                font-family: "Libre Franklin", sans-serif;
                text-decoration:underline;
                bottom: -50px;
            }

            .description-DR
            {
                position: relative;
                background-color:gray ;
                bottom: -55px;
                left: 770px;
                cursor:alias;
                width: fit-content;
                height: fit-content;
            }

            .description-text-DR
            {
                visibility: hidden;
                width: 800px;
                height: fit-content;
                background-color: #333;
                color: #fff;
                text-align: center;
                border-radius: 6px;
                padding: 10px;
                position: absolute;
                z-index: 1;
                bottom: 125%;
                left: 50%;
                margin-left: -200px;
                margin-bottom: 15px;
                opacity: 0;
                transition: opacity 2s;
            }

            .description-DR:hover .description-text-DR
                {
                visibility: visible;
                opacity: 20;
                }

            .E
            {
                color: white;
                position:absolute;
                font-size:30px;
                font-style:italic;
                font-weight: bold;
                left: 910px;   
                bottom: -62px;
                font-family:BeauRivage,courier;
                text-shadow: -20px 18px 8px red; 
            }

            nav .Web
            {
                background-color: red;
                position:absolute;
                left: 1088px;
                font-family: "Libre Franklin", sans-serif;
                text-decoration:underline;
            }

            .by
            {
                background-color: red;
                position:absolute;
                left: 1185px;
                font-family: "Libre Franklin", sans-serif;
                text-decoration:underline;
            }

            .description-Eng
            {
                position: relative;
                background-color:gray ;
                bottom: -24px;
                left: 1224px;
                cursor:alias;
            }

            .description-text-Eng
            {
                visibility: hidden;
                width: 280px;
                background-color: #333;
                color: #fff;
                text-align: center;
                border-radius: 6px;
                padding: 5px;
                position: absolute;
                z-index: 1;
                bottom: 125%;
                left: 50%;
                margin-left: -150px;
                margin-bottom: 15px;
                opacity: 0;
                transition: opacity 2s;
            }

            .description-Eng:hover .description-text-Eng
                {
                visibility: visible;
                opacity: 20;
                }

            .r
            {
                background-color:gray ;
                position:absolute;
                bottom: -48px;
                left: 1360px;
            }

            .FACEico
            {
                position:fixed;
                width:67px ;
                height:72px;
                bottom: 5px;
                left: 1430px; 
            }


            .A_M
            {
                background-image:url("BG_Main.jpg");
                background-repeat: no-repeat;
                background-attachment:scroll;
                background-size:cover;
                background-position: center;
                width: 98.38%;
                float: left;
                border: solid black;
                padding: 10px;
                font-size: 25px;
                color: white;
            }

            aside
            {
                text-align:center;
                width: 480px;
                float: left;
                clear: both;
                border:2px solid gray;
                padding: 10px;
                font-size: 20px;
                color: white;
                background-image:url("BG_Form.jpg");
                background-repeat: no-repeat;
                background-attachment:scroll;
                background-size:cover;
                background-position: center;
            }

            h3
            {
                color: darkmagenta;
                text-align: center;
                font-weight:bold;
                font-family:RubikDoodleShadow,courier;
                text-shadow: 20px 20px 16px red ;
                position: relative;
                bottom: 15px;
            }

            .LogoSide
            {
                position:relative;
                width: 334px;
                height: 332px;
                bottom: 20px; 
            }

            label
            {
                font-weight:bold;
                text-shadow: 20px 20px 16px red;
                position: relative;
                bottom: 10px;
                left: -15px;
                font-family: "LibreBaskerville",sans-serif;
            }

            .L_ID
            {
                position: relative;
                left: 3px; 
            }

            input
            {
                padding: 5px;
                border:1.9px solid white;
                text-align: left;
                font-size:17px;
                background-color: darkgrey;
                color: black;
                font-weight:bold;
                bottom: 10px;
                width: 250px;
            }

            .inputID
            {
                position: relative;
                left: 84px;
            }

            .GRN_ID
            {
                position: relative;
                bottom: 10px;
                border:1.9px solid crimson;
                font-size:17px;
                left: 85px; 
            }

            .inputFirst_Name
            {
                position: relative;
                left: 26px;
            }

            .inputLast_Name
            {
                position: relative;
                left: 28px;
            }

            .inputDate
            {
                position: relative;
                left: 60px;
            }

            .inputAddress
            {
                position: relative;
                left: 47px;
            }

            .inputPhone
            {
                position: relative;
                left: 54px;
            }

            .inputEmail
            {
                position: relative;
                left: 54px;
            }

            .inputSpecialization
            {
                position: relative;
                left: 17px;
                height: 34px;
                bottom: 10px;
                width: 55%;
                padding: 5px;
                border:1.9px solid white;
                text-align: left;
                font-size:17px;
                background-color: darkgrey;
                color: black;
                font-weight:bold;
            }
            
            .L_Gender
            {
                position: relative;
                left: 8px;
            }

            .inputMale
            {
                position: relative;
                left: -20px;
                cursor: pointer;
            }

            .L_Male
            {
                position: relative;
                left: -140px;
                font-family:RubikDoodleShadow,courier;
                text-shadow: 00px 00px 0px red;
            }

            .inputFemale
            {
                position: relative;
                bottom:34px;
                left: 135px;
                cursor: pointer;
            }

            .L_Female
            {
                position: relative;
                bottom:34px;
                left: 15px;
                font-family:RubikDoodleShadow,courier;
                text-shadow: 00px 00px 0px red;
            }

            button
            {
                padding: 5px;
                border:1.9px solid white;
                font-size:17px;
                font-weight: bold;
                background-color: darkgray;
                color: black;
                cursor: pointer;
            }

            .buttonADD
            {
                position: relative;
                left:-50px;
            }

            .buttonDELETE
            {
                position: relative;
                left:-25px;
            }
            

            .buttonCLEAR
            {
                position: relative;
                left: 50px;
            }

            .buttonUPDATE
            {
                position: relative;
                left: 25px;   
            }

            .DAS
            {
                position: relative;
                /* left: 65px;
                top: -20px;  */
                
            }

            main 
            {
                float: right;
                border: 10px solid gray;
                padding: 3px;
                border-top:10px  maroon;
                position: static;
                left: 20px;
                border-style:ridge;
            }

            .tbl
            {
                font-size: 20px;
                text-align: center;
                margin:3px;
            }

            .tbl th
            {
                color: red;
                font-size:20px;
                padding:2px;
                width : 88px;

            }

            td
            {
                height: 50px;
                word-break:break-all;
            }
        </style>
    </head>

    <body dir="ltr">
    <?php
        // connect with data base
        $host='localhost';
        $user='root';
        $pass=' ';
        $db='students_ohi';
        $con=mysqli_connect($host, $user, $pass, $db);
        $res=mysqli_query($con,"select * from students_ohi_t");

        // Check connection
        if ($con->connect_error)
        {
            die("Connection failed:".$con->connect_error);
        }

        //button variables , variabel names= same names in database > students
        $ID =' ';
        $First_Name =' ';
        $Last_Name =' ';
        $Date =' ';
        $Address =' ';
        $Phone =' ';
        $Email =' ';
        $Specialization =' ';
        $Gender =' ';

        if(isset($_POST['ID'])) 
        {
            $ID=$_POST['ID'];
        }

        if(isset($_POST['First_Name'])) 
        {
            $First_Name=$_POST['First_Name'];
        }

        if(isset($_POST['Last_Name'])) 
        {
            $Last_Name=$_POST['Last_Name'];
        }

        if(isset($_POST['Date'])) 
        {
            $Date=$_POST['Date'];
        }

        if(isset($_POST['Address'])) 
        {
            $Address=$_POST['Address'];
        }

        if(isset($_POST['Phone'])) 
        {
            $Phone=$_POST['Phone'];
        }

        if(isset($_POST['Email'])) 
        {
            $Email=$_POST['Email'];
        }

        if(isset($_POST['Specialization'])) 
        {
            $Specialization=$_POST['Specialization'];
        }

        if(isset($_POST['Gender'])) 
        {
            $Gender=$_POST['Gender'];
        }

        $sql=' ';
        if(isset($_POST['ADD']))
        {
            $sql="insert into students_ohi_t values('$ID','$First_Name','$Last_Name','$Date','$Address','$Phone','$Email','$Specialization','$Gender')";
            mysqli_query($con,$sql);
            echo '<meta http-equiv="refresh" content="0">';
        }

        if(isset($_POST['DELETE']))
        {
            $sql="delete from  students_ohi_t where First_Name='$First_Name'";
            mysqli_query($con,$sql);
            echo '<meta http-equiv="refresh" content="0">';
        }

        if (isset($_POST["DeleteAllStudents"])) 
        {
        $sql = "DELETE FROM students_ohi_t";
            if ($con->query($sql) === TRUE) 
            {
                echo '<meta http-equiv="refresh" content="0">';
            } 
            else
            {
                echo "Error deleting data:".$con->error;
            }
        }
        $con->close();
        ?>

        <header>
            <a href="https://www.ohie.edu.eg/ar" target="_blank" title="go to OHI"><img src="logoOHI.jpg" alt="will not show"/> </a>
            <p class="h1">"Obour Higher Institute For Engineering And Technology"</p>
        </header>

        <nav>
            <a href="https://www.ohie.edu.eg/ar" target="_blank" title="go to OHI"><img src="logoOHI.ico" alt="will not show" class="OHIico" /></a>
            <p class="Sup">Supervisor:</p>

            <div class="description-DR">
            Dr.Safaa
            <div class="description-text-DR">
                <img src="safaa.jpg" alt="will not show" width="280px" height="400px">   <br> 
                info :Professor at 'ASU' , former head of computer department in science college and currently Head of the Educational Technology Department 
                , Director and founder of the E-Learning Center and the Quality Unit and 'IT' at 'ASU' , She holds many awards including the Ideal Mother Award from the 'WHO' ,Supervising more than 60 scientific and research papers.</div>
            </div>

            <p class="Web">Website</p>
            <p class="by">By:</p>

            <div class="description-Eng">
            Eng.Eslam
            <div class="description-text-Eng"> 
                <!-- <img src="eslam.jpg" alt="will not show" width="250px" height="310px">   <br>   -->
                <img src="eslam2.jpg" alt="will not show" width="240px" height="330px">   <br>
                info : 5th Year At 'OHI' For Engineering and Technology, Department of Electricity, specializing in Computers.</div>
            </div>

            <p class="r">Reda</p>
            <P class="E">ESLAM</P>
            <a href="https://www.facebook.com/ohi1996/" target="_blank" title="go to OHI"><img src="facebook.ico" alt="will not show" class="FACEico" /></a>
        </nav>

        <div class="A_M">
            <form method="POST">
                <aside>
                    <div id="div_A"> 
                        <!--Control panel for managing students-->   
                        <h3>Students Management</h3>                                                                                                                              
                        <a href="https://www.ohie.edu.eg/ar" target="_blank" title="go to OHI"><img src="imageOHI.png" alt="will not show" class="LogoSide"/></a>                 <br>
                        <label for="ID" class="L_ID">ID</label>
                        <input type="number" name="ID" id="ID" class="inputID" placeholder="random ID" maxlength="11" required readonly/>  
                        <button type="button" onclick="generateRandomNumber()" class="GRN_ID" ><s style="font-weight:bold;" title="Click to add a random ID">&#8629;</s></button> <br><br>   

                        <label for="First_Name">First_Name</label>
                        <input type="text" name="First_Name" id="First_Name" class="inputFirst_Name" placeholder="enter your first name" maxlength="20" required/>                <br><br>

                        <label for="Last_Name">Last_Name</label>
                        <input type="text" name="Last_Name" id="Last_Name" class="inputLast_Name" placeholder="enter your last name" maxlength="20"/>                             <br><br>

                        <label for="da">Date</label>
                        <input type="date" id="da" name="Date" class="inputDate" placeholder="Enter your date of birth">                                           <br><br>

                        <label for="Address">Address</label>
                        <input type="text" name="Address" id="Address" class="inputAddress" placeholder="enter your address" maxlength="50"/>                                     <br><br>

                        <label for="Phone">Phone</label>
                        <input type="number" name="Phone" id="Phone" class="inputPhone" placeholder="enter number phone" maxlength="15"/>                                         <br><br>

                        <label for="Email">Email</label>
                        <input type="email" name="Email" id="Email" class="inputEmail" placeholder="enter your email" maxlength="30"/>                                            <br><br>

                        <label for="Specialization">Specialization</label>
                        <select name="Specialization" id="Specialization" class="inputSpecialization">           
                            <option value="General" selected>General</option>
                            <option value="Civil">Civil</option>
                            <option value="Architecture">Architecture</option>
                            <option value="Electricity">Electricity</option>
                            <optgroup label="Electricity">
                                <option value="Communications">Communications</option>
                                <option value="Computers">Computers</option> 
                            </optgroup>
                        </select>                                                                                                             <br><br>

                        <label class="L_Gender">Gender</label>
                        <input type="radio" name="Gender" value="Male" id="m" class="inputMale"> 
                        <label class="L_Male"for="m">Male</label>
                        <input type="radio" name="Gender" value="Female" id="fe" class="inputFemale">  
                        <label class="L_Female" for="fe">Female</label>                                                                                                           <br>

                        <button name="ADD" class="buttonADD" title="Add student">ADD</button>
                        <button name="DELETE" class="buttonDELETE" title="Delete student">Delete</button>                                                             
                        <button onclick="showWarning()" name="DeleteAllStudents" class="DAS" title="Delete all students from the data base">Delete All</button>          
                        <button onclick="refreshPage()" name="UPDATE" class="buttonUPDATE" title="Updating data">Update</button>   
                        <button type="reset" name="CLEAR" class="buttonCLEAR" title="Delete the entered data">Clear</button>                                                      <br><br>  
                    </div>
                </aside>

                <main>
                    <table border="4" class="tbl">
                        <tr>
                            <th>ID</th>
                            <th>First_Name</th>
                            <th>Last_Name</th>
                            <th>Date</th>
                            <th>Address</th>
                            <th>Phone</th>
                            <th>Email</th>
                            <th>Specialization</th>
                            <th>Gender</th>
                        </tr>

                        <?php
                        while($row=mysqli_fetch_array($res)) 
                        {
                            echo "<tr>";
                            echo "<td>".$row['ID']."</td>";
                            echo "<td>".$row['First_Name']."</td>";
                            echo "<td>".$row['Last_Name']."</td>";
                            echo "<td>".$row['Date']."</td>";
                            echo "<td>".$row['Address']."</td>";
                            echo "<td>".$row['Phone']."</td>";
                            echo "<td>".$row['Email']."</td>";
                            echo "<td>".$row['Specialization']."</td>";
                            echo "<td>".$row['Gender']."</td>";
                            echo "</tr>";
                        }
                        ?>
                    </table>
                </main>
            </form>
        </div>
    </body>
</html>