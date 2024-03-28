<div class="posts">
    <aside>
        <h3>
            posts
        </h3>
        <nav>

            <ul>
                <li>
                   <a href="/posts/one">one</a> 
                </li>
                <li>
                    <a href="/posts/2">2</a> 
                 </li>
                 <li>
                    <a href="/posts/3">3</a> 
                 </li>
            </ul>
        </nav>
    </aside>
    <main>
        <slot/>
    </main>
</div>

<style>
    .posts{
        display: grid;
        margin-top: 2rem;
        gap: 2rem;
        grid-template-columns: 200px 60ch;
    }
</style>