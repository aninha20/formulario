# formulario 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://unpkg.com/feather-icons"></script>
    <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
    <link rel="stylesheet" href="formulario.css">
    <title>Sign</title>
</head>
<body>
    <div class="form-container">
     <form>
        <h3>SIGN IN</h3>
        <div class="input-container">
            <input type="text" placeholder="User Name">
            <i data-feather="user"></i>
        </div>
        <div class="input-container">
            <input type="password" placeholder="Password">
            <i data-feather="lock"></i>
        </div>
        <div class="options-container">
            <div class="checkbox-container">
                <input type="checkbox" name="remember" id="remember">
                <label for="remember">Remember Me</label>
            </div><a href="www.google.com.br">Reset Password</a>
        </div>
        <input type="submit" value="Sign">

        <p>Or Sing in whith</p>
        <div class="social-media-container">
            <div class="icon-container">
                <i data-feather="facebook"></i>
            </div>
            <div class="icon-container">
                <i data-feather="mail"></i>
            </div>
            <div class="icon-container">
                <i data-feather="twitter"></i>
        </div>
        </div>
     <hr>
     <p class="footer">Do not have an account! <a href="google.com">Sing Up Now</a></p>
     </form>
    </div>

    <script>
        feather.replace()
    </script>

</body>
</html>

*/formulario css*/

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@500&display=swap');

body {
    font-family: 'Roboto', sans-serif;
    margin: 10;
    background-color: aliceblue;

}

* {
    box-sizing: border-box;
}

.form-container {
    background: white;
    margin: 15px auto;
    width: 400px;
    border-radius: 50px;
}

form {
    padding: 20px;
}

form .input-container {
    position: relative;
    margin-bottom: 15px;
}

form h3 {
    text-align: center;
}

form .input-container input, input[type='submit']{
    width: 100%;
    height: 45px;
    border-radius: 25px;
}

form input[type='submit']{
    border: 0;
    background-color: red;
    color: white;
    font-weight: bold;
    margin-bottom: 20px;
}

form .input-container input{
    border: 1px solid #e4e4e4;
    color: #818181;
    padding: 0 55px 0 25px;
    font-size: 1rem;
}

svg {
    position: absolute;
    right: 20px;
    top: calc(50% - 12px);
    color: #818181;
}

.options-container {
    padding: 0 20px;
    margin: 25px auto;
    color: #818181;
}

.options-container .checkbox-container {
    display: inline-block;
    width: 50%;
}

a {
    text-align: right;
    color: red;
    text-decoration: none;
    font-weight: bold;

}
form p{
    color: #818181 ;
    text-align: center;
}
form .social-media-container {
    margin: 20px auto;
    width: fit-content;
}
form .social-media-container .icon-container {
    background: #375c98; 
    display: inline-block;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    position: relative;


}
form .social-media-container .icon-container:nth-child(2){
    background: #c54f33;

}

form .social-media-container .icon-container:nth-child(3){
    background: #4dadf2;

}

form .social-media-container .icon-container svg{
    position: absolute;
    top: calc(50% - 12px);
    left: calc(50% - 12px);
    color: white;

}

.footer{
   width: fit-content;
    margin: 20px auto;
}
