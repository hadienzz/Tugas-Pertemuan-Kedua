<template>
    <div class="container">
        <nav>
              <ul>
                  <li><router-link to="/indexWeb">Home</router-link></li>
                  <li><router-link to="/loginForm">Login</router-link></li>
                  <li><router-link to="/random">Random</router-link></li>
              </ul>
          </nav>
          
        <div class="content">
            <h2>Color</h2>
            <p>Your World!</p>
            <button>try now</button>
        </div>
    </div>
</template>

<style>
body{

    margin: 0;
    padding: 0;
    height: 100vh;
    background-size: cover;
    background-position-x: 50%;
    background-position-y: 50%;
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}

.container{
    height: 100vh;
    width: 100%;
}

.content{
    width: 450px;
    height: 450px;
    background-color: white;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
    box-shadow: 0px 20px 20px rgba(0, 0, 0, 0.4), 
    0px 20px 20px rgba(0, 0, 0, 0.2),
    0px 0px 0px 20px rgba(67, 64, 234, 0.1),
    inset 0px 0px 0px 1px rgba(255, 255, 255, 1),
    inset 0px 0px 0px 1px rgba(67, 64, 234, 0.1);
}

.content h2{
    color: #4340ea;
    font-size: 140px;
    padding: 0;
    margin: 0;
    font-weight: 700;
}

.content p{
    color: black;
    font-size: 32px;
    font-weight: 650;
    letter-spacing: 1px;
    margin-top: -4px;
}

.content button{
    width: 140px;
    height: 50px;
    color: white;
    background-color: #4340ea;
    border: none;
    font-size: 20px;
    font-weight: 700;
    letter-spacing: 2px;
    cursor: pointer;
}

.content button:hover{
    background-color: #302df1;
}
</style>