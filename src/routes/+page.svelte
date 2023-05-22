<script>
    import ListItem from "$lib/ListItem.svelte";

    const items = [
        { title: "Amanita Muscaria", category: "Species", image: "https://www.naturezadivina.com.br/media/wysiwyg/pode-comer-amanita-muscaria.jpg" },
        { title: "Amanita Phalloides", category: "Species", image: "https://encrypted-tbn2.gstatic.com/licensed-image?q=tbn:ANd9GcSjfmn3dnqwqbz-trVZPIF4nX9SIVKGJxa0wfVjQ1CJAx9-zUmHuEXmvMKdhfI4veqUrzFxce1MhFjEkLA" }
        ];
</script>

{#each items as {title, category, image}}
    <ListItem {category} {title} {image}></ListItem>
{/each}
