<template>
    <div class="about">
        <h1>{{ pagename }}</h1>
        <p>{{ pagedescreption }}</p>
    </div>
</template>

<script>
// @ is an alias to /src

export default {
    data: function () {
        return {
            pagename: "About Us",
            pagedescreption: "Welcom TO About Us Page",
        };
    },
    name: "AboutView",
};
</script>
