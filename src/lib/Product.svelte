<script>
    import { Button } from 'flowbite-svelte';
    export let item;
    let i;
    $: i = {...item}
</script>

<div class="relative rounded-3xl shadow p-2">
<img class="px-8 pt-8 pb-2" src="/breakfast.jpg" alt="">
<p class="text-center text-xl font-semibold capitalize">Steak dishes.</p>
<p class="text-center">Lorem ipsum dolor. Sit, amet.</p>
<p class="pt-2 pb-8 text-center font-semibold text-lg text-yellow-300 dark:text-white">$9.99</p>
    <div class="absolute bottom-9 right-8">
    <Button pill={1} class="!p-2" color={"yellow"} on:click={() => console.log('click')} >
        <svg aria-hidden="true" class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path d="M3 1a1 1 0 000 2h1.22l.305 1.222a.997.997 0 00.01.042l1.358 5.43-.893.892C3.74 11.846 4.632 14 6.414 14H15a1 1 0 000-2H6.414l1-1H14a1 1 0 00.894-.553l3-6A1 1 0 0017 3H6.28l-.31-1.243A1 1 0 005 1H3zM16 16.5a1.5 1.5 0 11-3 0 1.5 1.5 0 013 0zM6.5 18a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path></svg>
    </Button>
    </div>
</div>