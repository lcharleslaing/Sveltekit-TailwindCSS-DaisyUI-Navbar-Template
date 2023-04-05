<script>
    import PageTitle from "$lib/components/PageTitle.svelte";
    import { goto } from "$app/navigation";
    import Card from "../../lib/components/Card.svelte";
</script>

<PageTitle customTitle="Applications" />

<div
    class="flex flex-col md:flex-row items-center justify-center mt-6 space-y-4 md:space-y-0 md:space-x-4"
>
    <Card
        href="#"
        iconName="youtube"
        title="Sample 1"
        description="Sample 1 Description"
    />
    <Card
        href="#"
        iconName="facebook"
        title="Sample 2"
        description="Sample 2 Description"
    />
    <!-- Add more Card components here -->
</div>
