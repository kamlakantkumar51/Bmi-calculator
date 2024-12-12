# Bmi-calculator
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bmi Calculator</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

    <div class="container">
        <h2>BMI Calculator</h2>
        <form id="bmiForm">

            <label for="gender">Gender:</label>
            <select id="gender" required>
                <option value="male">Male</option>
                <option value="female">Female</option>
            </select>
            <label for="age">Age:</label>
            <input type="number" id="age" placeholder="Enter Age " required>

            <label for="height-feet">Height:</label>
            <input type="number" id="height-feet" placeholder="Feet"required>
            <input type="number" id="height-inches" placeholder="Inches" required>

            <label for="weight">Weight:</label>
            <input type="number" required id="weight" placeholder="Enter Weight in kg">

            <input type="submit" value="Calculate BMI">
        </form>

        <div id="result"></div>
    </div>



    <script src="script.js"></script>
</body>

</html>




body{
    background-color: blue;
}

.container{
    max-width: 400px;
    margin: 200px auto;
    padding: 20px;
    background-color: #f2f2f2;
    border:2px solid #1e5f8a;
    border-radius: 2px 10px 10px rgba(0,0,0,0.2 );
}
h2{
    margin-top: 0;
    text-align: center;
    text-decoration: underline;

}
form{
    margin-bottom: 20px;
    display: flex;
    flex-direction: column;
}
label{
    font-size: large;
    font-weight: 600px;
    margin-bottom: 5px;
    color: #000;
}
input[type="number"],
select{
    width: 95%;
    padding: 10px;
    border: none;
    background:#fff;
    border-radius: 5px;
    box-shadow: 0px 0px 5px rgba(0,0,0,0.2);
    margin-bottom: 10px;
}
input[type="number"]:focus,
select:focus{
    outline: none;
    box-shadow: 0px 0px 5px #3498db;
}
select{
    width: 100%;

}
input[type="submit"]{

    padding: 10px;
    margin-top: 10px;
    background-color: blue;
    border: none;
    border-radius: 3px;
    color: #fff;
    cursor: pointer;
    transition: background-color 0.s ease;


}
input[type="submit"]:hover{
    background-color: blue;
}
#result{
    font-weight: bold;
    margin-top: 20px;
    color: blue;
}


