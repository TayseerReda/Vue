<template>
    <div>
        <h1>{{ pagename }}</h1>
        <p>{{ pagedescreption }}</p>
        <post-blog
            v-for="post in posts"
            v-bind:key="post.id"
            :view="post.view"
            :title="post.title"
            :date="post.date"
            :content="post.content"
            :auther="post.auther"
            :category="post.category"
        />
    </div>
</template>
<script>
import JsonPosts from "../json/JsonPosts.json";
import PostBlog from "@/components/Blog/PostBlog.vue";

export default {
    data: function () {
        return {
            pagename: "Blog",
            pagedescreption: "Welcom TO Blog Page",
            posts: JsonPosts,
        };
    },
    name: "BlogView",
    components: {
        PostBlog,
    },
};
</script>
