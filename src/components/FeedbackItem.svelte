<script>
    import Card from "./Card.svelte";
    export let item;
</script>
<Card>
    {item.id}
    {item.text}
    {item.rating}
</Card>