<template>
    <div class="app">
        <nav
            class="bg-gradient-to-r from-orange-400 to-red-600 flex items-center w-full h-16 px-5 mb-5"
        >
            <h1 class="text-4xl text-white font-bold mr-6">Blog Akawam</h1>
            <ul>
                <li>
                    <nuxt-link to="/"
                               class="text-sm bg-gray-200 py-1 px-3 rounded-lg font-semibold hover:bg-red-600 hover:text-white">
                        Accueil
                    </nuxt-link>
                </li>
            </ul>
        </nav>
        <div class="posts mx-auto max-w-6xl">
            <h2 class="text-4xl text-gray-800 font-bold mb-4 border-b">Articles</h2>
            <div class="post bg-gray-200 py-1 px-3 rounded mb-10 border"
                 v-for="post in post">
                <h3 class="text-3xl font-bold text-red-600">{{ post.subject }}</h3>
                <p class="py-2 mb-2 px-1">
                    {{ post.content }}
                </p>
                <div class="flex justify-center -mb-4">
                    <nuxt-link to="/"
                               class="bg-gradient-to-r from-orange-400 to-red-600 rounded-md text-white font-semibold py-1 px-6 hover:from-red-600">
                        Voir l'article
                    </nuxt-link>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    async asyncData({ $axios }){
        let {data:posts} = $axios.get('/api/posts');
        console.log('POSTS',posts);
        return {
            posts:posts
        }
    },
}
</script>
