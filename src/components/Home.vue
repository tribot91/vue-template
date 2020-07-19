<template>
    <div class="home p-5">
        <b-row>
            <b-col cols="4">
                <b-dropdown id="dropdown-1" text="Dropdown Button" class="m-md-2">
                    <b-dropdown-item>First Action</b-dropdown-item>
                    <b-dropdown-item>Second Action</b-dropdown-item>
                    <b-dropdown-item>Third Action</b-dropdown-item>
                    <b-dropdown-divider></b-dropdown-divider>
                    <b-dropdown-item active>Active action</b-dropdown-item>
                    <b-dropdown-item disabled>Disabled action</b-dropdown-item>
                </b-dropdown>
            </b-col>
            <b-col cols="8">
                <b-input-group size="lg" prepend="$" append=".00"> <b-form-input></b-form-input> </b-input-group>
            </b-col>
        </b-row>
        <b-row>
            <hr />
        </b-row>
    </div>
</template>

<style lang="scss" scoped>
.home {
    background: white;
    border-radius: 5px;
}
#dropdown-1 {
    height: 100%;
    width: 100%;
    margin: 0 !important;
}
</style>
