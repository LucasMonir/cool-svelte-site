<script>
        import {page} from "$app/stores";
        const links = [
                { name: "Home", route: "/" },
                { name: "About", route: "/about" },
                { name: "Contact", route: "/contact" },
                { name: "Doubts", route: "/doubts" },
        ];
        const normalClass =
                "text-gray-800 transition-colors duration-300 transform dark:text-gray-200 mx-1.5 sm:mx-6 ";
        const activeClass = normalClass + "border-b-2 border-blue-500";
</script>

{#each links as { name, route }}
        <a href={route} class={$page.url.pathname === route ? activeClass : normalClass}>{name}</a>
{/each}
