<template>
    <div id="email-field">
        <div class="form-group">
            <label for="email">Correo</label>
            <input type="email" id="email" class="form-control" name="email" placeholder="Tu correo" required>
            <div class="invalid-feedback">
                <div>Correo electrónico es requerido.</div>
                <div>El email debe ser válido.</div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "EmailField"
    }
</script>

<style scoped>
    
</style>