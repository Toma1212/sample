<template>
    <nav class="navbar">
        <RouterLink class="navbar_brand" to="/">
            Laravel x Vue
        </RouterLink>
        <div class="navbar_menu">
            <div class="navbar_item">
                <b-button variant="primary">
                    Submit
                </b-button>
            </div>
            <span class="navbar_item">
                username
            </span>
            <div class="navbar__item">
                <RouterLink class="btn btn-primary" to="/login">
                    Login / Register
                </RouterLink>
            </div>
        </div>
    </nav>
</template>

<script>
export default {

}
</script>