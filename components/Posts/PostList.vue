<template>
    <div>
        <section class="post-list">
            
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

    .posts-page {
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>