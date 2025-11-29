<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Login - Student Support Portal</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
    body {
        margin: 0;
        padding: 0;
        font-family: Arial, sans-serif;
        background: #0e1a2b;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        color: #fff;
    }

    .login-box {
        width: 360px;
        background: rgba(255,255,255,0.08);
        padding: 30px;
        border-radius: 12px;
        box-shadow: 0 0 20px rgba(0,0,0,0.4);
        text-align: center;
    }

    .login-box h2 {
        color: #9ec5ff;
        margin-bottom: 25px;
    }

    .login-box input {
        width: 100%;
        padding: 12px;
        margin: 10px 0;
        border-radius: 8px;
        border: none;
        outline: none;
        font-size: 15px;
        background: rgba(255,255,255,0.12);
        color: white;
    }

    .btn-login {
        width: 100%;
        background: #6c4bff;
        border: none;
        padding: 12px;
        font-size: 16px;
        color: white;
        margin-top: 15px;
        border-radius: 8px;
        cursor: pointer;
    }

    .btn-login:hover {
        background: #5836e2;
    }

    .small-text {
        margin-top: 10px;
        opacity: 0.7;
        font-size: 14px;
    }
</style>
</head>
<body>

<div class="login-box">
    <h2>Student Login</h2>

    <input type="text" id="username" placeholder="Enter Username">
    <input type="password" id="password" placeholder="Enter Password">

    <button class="btn-login" onclick="login()">Login</button>

    <p class="small-text">Your information stays private & secure.</p>
</div>

<script>
function login() {
    let user = document.getElementById("username").value.trim();
    let pass = document.getElementById("password").value.trim();

    if (user === "" || pass === "") {
        alert("Please enter username and password");
        return;
    }

    window.location.href = "Health.html";
}
</script>

</body>
</html>
