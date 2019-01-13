<template>
    <div id="signin-form">
        <div id="authentication_box">
            <h3 id="form_tittle">Iniciar sesión</h3>
            <span id="explanatory_message">
                        <small class="form-text text-muted">
                            Para acceder a tu cuenta debes contar con tu correo y contraseña.
                        </small>
                    </span>
            <form id="authentication_form">
                <email-field></email-field>
                <div class="form-group">
                    <label for="password">Constraseña</label>
                    <input type="password" name="password" id="password" class="form-control" placeholder="Contraseña" required minlength="8">
                    <div class="invalid-feedback">
                        <div>La contraseña es requerida.</div>
                        <div>La contraseña debe tener un mínimo de 8 carácteres.</div>
                    </div>
                </div>
                <button type="submit" class="btn btn-success">Iniciar sesión</button>
            </form>
            <div class="alert alert-danger" role="alert">
                <p >-error</p>
            </div>
        </div>
    </div>
</template>

<script>
    import EmailField from "./UI/EmailField";

    export default {
        name: "SigninForm",
        components:{
            EmailField
        }
    }
</script>

<style scoped>
    #explanatory_message{
        text-align: center;
    }

    #authentication_box{
        border: rgb(209, 209, 209) 1px solid;
        border-radius: 10px;
        padding: 20px;
        margin:auto;
        width: 400px;
    }

    #form_tittle{
        text-align: center;
    }

    #authentication_form{
        margin: 5px;
    }
</style>