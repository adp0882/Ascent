<?php

$servername "localhost";
$username "root";
$password "";
$dbname= "StudentRecord";

$conn=new mysqli($servername,$username,$password,$dbname);

if ($conn->connection_error){
    die("Connection Failed" . $conn->connect_error);
}
else
    echo "Connected Succesfully.";

    $sql="Select * from studentInfo";
    $result=$conn->query("$sql");
    
    if ($result){
        while ($row=$result-> fetch_assoc()){
            echo "studentID" .$row ["studentId"]; ."<br>"
            . "Last Name:" .$row["lastName"] ."<br>"
            . "First Name" .$row["firstName"] ."<br>"
            . "Date of Birth" .$row["dateofbirth"] ."<br>"
            . "Email" .$row["email"] ."<br>"
            . "Phone number" .$row["phone"] ."<br>"
            ."<br>";
        }
    }
    else {
        echo "Error:" .$sql . "<br>" .$conn->error;
    }
 ?>
