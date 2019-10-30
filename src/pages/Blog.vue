<template>
  <Layout>
    <h1 class="my-4 font-weight-lighter mb-5 pb-5">Services</h1>

    <g-link
      :to="item.node.path"
      v-for="item in $page.posts.edges"
      :key="item.node.id"
      class="blog-post"
    >

    <div class="media">
      
      <div class="media-body">
        <g-image immediate :src="item.node.image" class="mb-2" alt="image" />
        <h5 class="mt-0">{{item.node.title}}</h5>
        <p class="text-light">{{item.node.excerpt}}</p>
        <div class="divider"></div>
      </div>
    </div>

    </g-link>
  </Layout>
</template>

<page-query>
query Blog {
	posts: allBlogPost(sortBy: "date") {
    edges {
      node {
        id
        path
        title
        excerpt
        image
      }
    }
  }
}
</page-query>

<style lang="scss" scoped>
.media {
  img {
    width: 120px;
    height: 120px;
  }
}

.media-body {
  margin: auto;
}
</style>
