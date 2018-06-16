<template>
<div class="home-page">
  <section class="intro">
    <h1>Awesome title here</h1>
  </section>
  <section class="featured-posts">
    
    <PostPreview
    id="1"
    thumbnail="http://via.placeholder.com/350x150"
    title="Hello there"
    previewText="This is my first post" >
    </PostPreview>
    <PostPreview
    id="2"
    thumbnail="http://via.placeholder.com/350x150"
    title="Another one?"
    previewText="This is my second post" >
    </PostPreview>
    <PostPreview
    id="3"
    thumbnail="http://via.placeholder.com/350x150"
    title="Yep another"
    previewText="This is my thid post" >
    </PostPreview>    
  </section>
</div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview';

export default {
  components: {
    PostPreview
  }
}
</script>


<style scoped>
.intro {
  height: 120px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 4px;
  box-shadow: 3px 4px 2px black;
  box-sizing: border-box;
  border: 1px solid peru;
  display: flex;
  justify-content: center;  
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

</style>
