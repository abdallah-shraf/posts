<template>
    <div class="our-blog">
        <h1>{{ pageName }}</h1>
        <p>{{ pageDesc }}</p>
        <div class="container">
            <div class="row">
                <div class="col-md-8">
                    <div class="posts-area">
                        <blog-bosts v-for="post in posts" 
                        :key="post.id"
                        :views="post.views"
                        :title="post.title"
                        :date="post.date"
                        :content="post.content"
                        :auther="post.auther"
                        :category="post.category"
                        />
                    </div>
                </div>
                <div class="col-md-4">
                    <blogSidbar/>
                </div>
            </div>
        </div>
    </div>
</template>
<script>

import blogBosts from "@/components/Blog/blogBosts.vue";
import blogSidbar from "@/components/Blog/blogSidbar.vue";
import jsonPosts from "../json/plog_posts.json";

export default {
  data: function () {
    return {
      pageName: "Blog Us",
      pageDesc: "This Is Blog Us Page",
      posts:jsonPosts,
    };
  },
  name: "blog",
  components: {
    blogBosts,
    blogSidbar
  }

};
</script>

