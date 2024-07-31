<template>
    <div>
        <h1>{{ pagename }}</h1>
        <p>{{ pagedescreption }}</p>
    </div>
</template>
<script>
export default {
    data: function () {
        return {
            pagename: "Help",
            pagedescreption: "Welcom TO Help Page",
        };
    },
    name: "HelpView",
};
</script>
