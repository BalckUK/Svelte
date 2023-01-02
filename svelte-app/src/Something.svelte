<script>
    import {onMount, onDestroy} from 'svelte'

    onMount(() => {
        console.log('Mounted!')
        return () => {
            console.log('Destory in mount')
        }
    })
    onDestroy(() => {
        console.log('Before destory~')
       /*  const h1 = document.querySelector('h1')
        console.log(h1.innerHTML) */
    })
</script>

<h1>Something...</h1>