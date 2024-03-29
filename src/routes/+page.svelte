<script lang="ts">
	import type { PageData } from "./$types";

    
export let data:PageData
$: ({posts}=data)
</script>

<h1>Posts</h1>

<p>Showing {posts.length} posts</p>

{#each data.posts as {slug,title}}
    <ul>
        <li>
            <a href="/posts/{slug}">{title}</a>
        </li>
    </ul>
{/each}