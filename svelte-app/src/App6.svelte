<script>
    let fruits=['Apple', 'Banana','Cherry', 'Orange', 'Mango']
</script>

<h2>
    Fruits
</h2>
<ul>
    {#each fruits as fruit}
    <li>{fruit}</li>
    {/each}
</ul>

<h2>
    Fruits reverse
</h2>
<ul>
    <!-- 
       ...['Apple', 'Banana','Cherry', 'Orange', 'Mango']
       'Apple', 'Banana','Cherry', 'Orange', 'Mango'
       ['Apple', 'Banana','Cherry', 'Orange', 'Mango']
    -->
    {#each [...fruits].reverse() as fruit}
    <li>{fruit}</li>
    {/each}
</ul>


<h2>
    Fruits slice -2
</h2>
<ul>
    {#each fruits.slice(-2) as fruit}
    <li>{fruit}</li>
    {/each}
</ul>