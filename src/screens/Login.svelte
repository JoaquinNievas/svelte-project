<script>
    function login() {
        console.log("Ingreso");
    }
</script>

<div class="fondo">
    <img src="assets/images/apperto.png" alt="logo" class="logo" />
    <div class="loginForm">
        <h5 class="password-title">CONTRASEÑA</h5>
        <input
            type="text"
            class="password-textfield"
            placeholder="Ingresá tu contraseña"
        />
        <button on:click={login} class="loginButton">Acceder</button>
    </div>

    <h6 class="version">V 2.0.0</h6>
</div>

<style>
    .fondo {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 100%;
        position: fixed;
        background-image: linear-gradient(#39a8ff, #397eff, #397eff);
    }

    .loginForm {
        width: 300px;
        height: 150px;
        margin-bottom: 50px;
        border-style: solid;
        border-color: white;
        border-radius: 20px;
        border-width: 1px;
        position: relative;
        overflow: hidden;
    }

    .logo {
        width: 150px;
        margin-bottom: 30px;
    }

    .version {
        color: white;
        position: absolute;
        bottom: 0%;
        margin-bottom: 1em;
    }

    .loginButton {
        position: absolute;
        bottom: 0%;
        color: #387aff;
        background-color: white;
        outline: none;
        border: none;
        height: 2.5em;
        width: 100%;
        cursor: pointer;
    }

    .password-title {
        margin-top: 20px;
        margin-left: 20px;
        color: white;
        font-size: 0.8em;
    }

    .password-textfield {
        position: absolute;
        margin-top: 20px;
        margin-left: 20px;
        background-color: transparent;
        color: white;
        outline: none;
        border: none;
    }

    ::-webkit-input-placeholder {
        color: rgba(255, 255, 255, 0.5);
    }
</style>
