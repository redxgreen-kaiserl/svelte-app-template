<script>
    import './app.css';
    import { route } from './lib/stores';

    let currentRoute = $route

    $: {
        currentRoute = $route
    }

</script>

{#if currentRoute === "home"}
    <div class="w-screen h-screen bg-black flex justify-center items-center">
        <p class="text-white">Hallo</p>
    </div>

{:else if currentRoute === "login"}
    login
{/if}