<template>
    <div class="post-box">
        <div class="row">
            <div class="card mt-5" style="width: 50%">
                <div class="card-body">
                    <div class="col-sm-12">
                        <h3 class="post-title" v-bold v-font="60">
                            {{ title }}
                        </h3>
                        <span class="post-date">Date: {{ date }}</span>
                        <p class="post-content">content: {{ content }}</p>
                        <div class="row">
                            <span class="post-views">views: {{ view }}</span>
                            <div class="col-sm-6">
                                <p class="post-author">auther: {{ auther }}</p>
                            </div>
                            <div class="col-sm-6">
                                <span>category: {{ category }}</span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "PostBlog",
    props: ["view", "title", "date", "content", "auther", "category"],
};
</script>
<style>
.row {
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
