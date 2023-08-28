<template>
    <div class="container">
            <nav>
                <ul>
                    <li><router-link to="/index">Home</router-link></li>
                    <li><router-link to="/loginForm">Home</router-link></li>
                    <li><a href="#">Home</a></li>
                </ul>
            </nav>
            <article>
                <div>
                <h2>Hallo!</h2>
                <p>Selamat Datang Di Website Saya, <br>
                    Salam Kenal!
                </p>
                </div>
                <div>
                    <img src="~/assets/headerImg.jpg" width="300px" height="300px" />
                </div>
            </article>
            <footer>
                <p>This Website created by Hadin Pramiadi. Copyright @2023</p>
            </footer>
    </div>
</template>

<style>
* {
    margin: 0;
    padding: 0;
}

.container {
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(to bottom left, orange, blue); 
}

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

article {
    display: flex;
    width: 100%;
    justify-content: space-evenly;
    margin: 100px 0;
    color: #9792e8;
    font-size: 30px;
}

article img {
    object-fit: cover;
    background-repeat: no-repeat;
    border-radius: 50px;
}

article h2 {
    color: #585a92;
    margin: 60px 0 30px 0;
    font-size: 70px;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

footer {
    color: #9792e8;
    width: 100%;
    position: absolute;
    bottom: 0;
    text-align: center;
    padding: 30px 0;
    display: flex;
    justify-content: center;
    align-items: center;
}


</style>