<!-- src/lib/components/PageTitle.svelte -->
<script>
    import { onMount } from "svelte";
    import Big2TinyLogo from "./Big2TinyLogo.svelte";

    let sitename = import.meta.env.VITE_WEBSITE_TITLE;

    let title = "";
    let isHomePage = false;
    export let customTitle;

    function capitalizeFirstLetter(string) {
        return string.charAt(0).toUpperCase() + string.slice(1);
    }

    onMount(() => {
        const pathname = window.location.pathname;
        isHomePage = pathname === "/";
        const routeName = isHomePage
            ? `sitename`
            : pathname.split("/").pop() || "Home";
        title =
            routeName === sitename
                ? routeName
                : capitalizeFirstLetter(routeName);
        if (customTitle) {
            title = customTitle;
        }
        document.title = title;
    });
</script>

<div class="text-center">
    <Big2TinyLogo />
    {#if !isHomePage}
        <h2 class="text-2xl font-extrabold uppercase mt-4">{title}</h2>
    {/if}
</div>
