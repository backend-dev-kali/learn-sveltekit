<script lang="ts">
	import type { PageData } from "./$types";

    export let data:PageData

    function formatDate(date:Date){
        return new Intl.DateTimeFormat('en',{dateStyle:'short'}).format(date)
    }
</script>

<hgroup>
    <h1>{data.post.title}</h1>
    <h2>{data.post.createdAt}</h2>

</hgroup>

<div class="content">
    {@html data.post.content}
</div>