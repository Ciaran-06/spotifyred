<script>
</script>

<div class="view">
    <ul class="circles">
        <li class="h1 item" />
        <li class="h2 item" />
        <li class="h3 item" />
        <li class="h4 item" />
        <li class="h5 item" />
        <li class="h6 item" />
        <li class="h7 item" />
    </ul>
</div>

<div id="content">
    <div id="login-container">
        <div class="login">
            <h1>Login</h1>
            <form action="http://192.168.1.136:7812/login">
                <input
                    type="submit"
                    id="login-button"
                    class="big-btn"
                    value="Log in with Spotify"
                />
            </form>
            <p class="login-desc">
                Please login to get access to spotify content.
            </p>
            <p class="login-desc-small">
                You will automatically be redirected to this page after login.
            </p>
        </div>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Varela+Round&display=swap');

    * {
        font-family: 'Varela Round', sans-serif;
    }
    h1 {
        font-size: 2em;
        margin-bottom: 12px;
        margin-top: 0;
    }

    #login-button {
        margin: 10px;
    }
    #content {
        display: -ms-flexbox;
        display: flex;
        -ms-flex-direction: column;
        flex-direction: column;
        position: absolute;
        top: 0;
        bottom: 0;
        right: 0;
        left: 0;
        overflow: hidden;
        background-color: #1db95442;
    }

    #login-container {
        display: -ms-flexbox;
        display: flex;
        height: 100%;
        -ms-flex-direction: column;
        flex-direction: column;
        -ms-flex-align: center;
        align-items: center;
        margin: 0 auto;
        -ms-flex-pack: center;
        justify-content: center;
    }

    #login-container .login {
        background-color: rgba(0, 0, 0, 0.5);
        color: #ffffff;
        text-align: center;
        padding: 70px;
    }

    #login-container .login .big-btn {
        margin: 10px 0 20px 0;
    }

    #login-container .login p {
        margin: 5px 0;
        font-size: 14px;
    }

    .big-btn {
        color: #fff;
        background-color: #1db954;
        font-size: 14px;
        line-height: 1;
        border-radius: 500px;
        padding: 18px 48px 16px;
        transition-property: background-color;
        transition-duration: 0.3s;
        border-width: 0;
        letter-spacing: 2px;
        min-width: 160px;
        text-transform: uppercase;
        white-space: normal;
        cursor: pointer;
    }

    .big-btn:hover {
        background-color: #1bd45c;
    }

    .view {
        position: absolute;
        width: 400px;
        height: 400px;
        top: 50%;
        left: 50%;
        margin: -200px 0 0 -200px;
    }

    .circles {
        height: 100%;
        margin: 0;
        padding: 0;
        transform-style: preserve-3d;
    }

    .item {
        position: absolute;
        top: 0;
        left: 0;
        list-style: none;
        padding: 0;
        border: 15px solid #cfd9db;
        border-radius: 50%;
        width: 400px;
        height: 200px;
        position: absolute;
        top: 0;
        left: 0;
        box-sizing: border-box;
    }

    .h1 {
        border: 15px solid #ccd7d9;
        border-color: #ccd7d9 #d2dbde #d7e0e2 #d2dbde;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #aebfc4,
            inset 0 10px 0px #aebfc4, 0 5px 0 #bdcbce, 0 10px 0 #bdcbce;
        width: 400px;
        height: 400px;
        transform: rotateX(70deg) translate3d(0px, 0px, -30px);
        animation: wave1 2s ease-in-out -0ms infinite alternate;
    }

    @keyframes wave1 {
        100% {
            transform: rotateX(70deg) translate3d(0px, 0px, 100px);
        }
    }
    .h2 {
        border: 15px solid #c9d4d7;
        border-color: #c9d4d7 #cfd9db #d5dde0 #cfd9db;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #abbdc1,
            inset 0 10px 0px #abbdc1, 0 5px 0 #bac9cc, 0 10px 0 #bac9cc;
        width: 340px;
        height: 340px;
        transform: rotateX(70deg) translate3d(30px, 0px, -60px);
        animation: wave2 2s ease-in-out -400ms infinite alternate;
    }

    @keyframes wave2 {
        100% {
            transform: rotateX(70deg) translate3d(30px, 0px, 70px);
        }
    }
    .h3 {
        border: 15px solid #c6d2d5;
        border-color: #c6d2d5 #ccd7d9 #d2dbde #ccd7d9;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #a8bbbf,
            inset 0 10px 0px #a8bbbf, 0 5px 0 #b7c6ca, 0 10px 0 #b7c6ca;
        width: 280px;
        height: 280px;
        transform: rotateX(70deg) translate3d(60px, 0px, -90px);
        animation: wave3 2s ease-in-out -800ms infinite alternate;
    }

    @keyframes wave3 {
        100% {
            transform: rotateX(70deg) translate3d(60px, 0px, 40px);
        }
    }
    .h4 {
        border: 15px solid #c3d0d3;
        border-color: #c3d0d3 #c9d4d7 #cfd9db #c9d4d7;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #a6b8bd,
            inset 0 10px 0px #a6b8bd, 0 5px 0 #b4c4c8, 0 10px 0 #b4c4c8;
        width: 220px;
        height: 220px;
        transform: rotateX(70deg) translate3d(90px, 0px, -120px);
        animation: wave4 2s ease-in-out -1200ms infinite alternate;
    }

    @keyframes wave4 {
        100% {
            transform: rotateX(70deg) translate3d(90px, 0px, 10px);
        }
    }
    .h5 {
        border: 15px solid #c0cdd1;
        border-color: #c0cdd1 #c6d2d5 #ccd7d9 #c6d2d5;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #a3b6bb,
            inset 0 10px 0px #a3b6bb, 0 5px 0 #b1c2c6, 0 10px 0 #b1c2c6;
        width: 160px;
        height: 160px;
        transform: rotateX(70deg) translate3d(120px, 0px, -150px);
        animation: wave5 2s ease-in-out -1600ms infinite alternate;
    }

    @keyframes wave5 {
        100% {
            transform: rotateX(70deg) translate3d(120px, 0px, -20px);
        }
    }
    .h6 {
        border: 15px solid #bdcbce;
        border-color: #bdcbce #c3d0d3 #c9d4d7 #c3d0d3;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #a0b4b9,
            inset 0 10px 0px #a0b4b9, 0 5px 0 #aebfc4, 0 10px 0 #aebfc4;
        width: 100px;
        height: 100px;
        transform: rotateX(70deg) translate3d(150px, 0px, -180px);
        animation: wave6 2s ease-in-out -2000ms infinite alternate;
    }

    @keyframes wave6 {
        100% {
            transform: rotateX(70deg) translate3d(150px, 0px, -50px);
        }
    }
    .h7 {
        border: 15px solid #bac9cc;
        border-color: #bac9cc #c0cdd1 #c6d2d5 #c0cdd1;
        box-shadow: 0 1px 0 white, inset 0 5px 0px #9db1b7,
            inset 0 10px 0px #9db1b7, 0 5px 0 #abbdc1, 0 10px 0 #abbdc1;
        width: 40px;
        height: 40px;
        transform: rotateX(70deg) translate3d(180px, 0px, -210px);
        animation: wave7 2s ease-in-out -2400ms infinite alternate;
    }

    @keyframes wave7 {
        100% {
            transform: rotateX(70deg) translate3d(180px, 0px, -80px);
        }
    }
</style>
