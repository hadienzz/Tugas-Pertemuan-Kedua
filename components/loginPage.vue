<template>
    <div class="container">
    <nav>
        <ul>
            <li><router-link to="/index">Home</router-link></li>
            <li><a href="/loginForm">Login</a></li>
            <li><a href="#">Home</a></li>
        </ul>
    </nav>
        <div class="form-field">
            <h1>Login Page</h1>
            <div class="text-field">
                <input type="text" placeholder="Username" id="username">
            </div>
            <div class="text-field">
                <input type="password" placeholder="Password" id="password">
                <div class="check">
                    <a href="#">Forgot Password?</a>
                    <div>
                        <input type="checkbox" name="" id="showPassword">
                        <label for="showPassword" id="textShowPassword">Show Password</label>
                    </div>
                </div>
            </div>
            <div class="text"></div>
            <div class="btn-login">
                <button>Login</button>
                <p>Not a member? <a href="#" class="link">Sign up</a></p>
            </div>
        </div>
    </div>
</template>

<style scoped>
nav {
    position: relative;
    top: 0;
    height: 80px;
    width: 100%;
    background-color: #9792e8;
    display: flex;
    align-items: center;
    justify-content: center;
}

nav ul {
    display: flex;
    gap: 120px;
}

nav ul li {
    display: inline-flex;
    justify-content: space-between;    
}

nav ul li a {
    color: #585a92;
    font-family: Arial, Helvetica, sans-serif;
    text-decoration: none;
}

* {
    margin: 0;
    padding: 0;
    font-family: 'Montserrat', sans-serif;
}


body {
    background-image: linear-gradient(to bottom left, orange, blue); 
    width: 100%;
    height: 100vh;
}

.form-field {
    width: 400px;
    height: 450px;
    background-color: #fff;
    border-radius: 15px;
    border: 2px solid silver;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
    box-sizing: border-box;
    color: #111;
    font-size: 12px;
    box-sizing: border-box;
    padding: 20px;
}

.form-field h1 {
    text-align: center;
    line-height: 100%;
    border-bottom: 1px solid silver;
    padding: 3px 0;

}

.form-field .text-field input {
    width: 100%;
    padding: 20px 0;
    border: none;
    overflow: auto;
    margin: 10px 0;
    border-bottom: 1px solid silver;
    outline: none;
    font-size: 16px;
}

.form-field .text-field input:active {
    border: none;
}


.text-field a {
    width: 100;
    height: 20px;
    font-size: 15px;
    text-decoration: none;
    display: inline-block;
    margin-top: 20px;
    margin-bottom: -20px;
}

.text-field a:hover {
    border-bottom: 1px solid blue;
} 

.btn-login {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 20px 0;
}


button {
    background-color: rgb(1, 132, 255);
    border: none;
    width: 200px;
    height: 50px;
    border-radius: 20px;
}

button:hover{
    background-color: rgb(0, 255, 157);
    cursor: pointer;
    transition: .2s;
}


.btn-login p, .btn-login a {
    font-size: 15px;
    text-decoration: none;
}

.btn-login a:hover {
    border-bottom: 1px solid blue;
}

.text {
    color: red;
    font-size: 16px;
    margin: 20px 0;
    width: 100%;
    height: 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-weight: bold;
}

.check {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

</style>