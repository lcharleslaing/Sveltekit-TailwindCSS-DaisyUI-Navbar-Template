<script>
    import NavbarMenuLinks from "./NavbarMenuLinks.svelte";

    let sitename = import.meta.env.VITE_WEBSITE_TITLE;
</script>

<div class="navbar bg-base-100 shadow-lg">
    <div class="navbar-start">
        <div class="dropdown">
            <!-- svelte-ignore a11y-no-noninteractive-tabindex -->
            <!-- svelte-ignore a11y-label-has-associated-control -->
            <label tabindex="0" class="btn btn-ghost lg:hidden">
                <!-- ... -->
            </label>
            <!-- svelte-ignore a11y-no-noninteractive-tabindex -->
            <ul
                tabindex="0"
                class="menu menu-compact dropdown-content mt-3 p-2 shadow bg-base-100 rounded-box w-52"
            >
                <!-- ... -->
                <NavbarMenuLinks />
            </ul>
        </div>
        <a href="/" class="btn btn-ghost normal-case text-xl">
            <img src="./icon.png" alt="Logo" class="inline h-6 w-6 mr-2" />
            {sitename}
        </a>
    </div>
    <div class="navbar-center hidden lg:flex w-full">
        <div class="flex justify-center w-full">
            <ul class="menu menu-horizontal px-1">
                <!-- svelte-ignore a11y-no-noninteractive-tabindex -->
                <!-- Insert Menu Links Here -->
                <NavbarMenuLinks />
            </ul>
        </div>
    </div>
</div>
<slot />
