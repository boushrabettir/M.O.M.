<script>
    import FeedbackItem from "./feedbackItem.svelte";
    export let feedback = [];
</script>

{#each feedback as fb (fb.id)}
   <FeedbackItem item = {fb} on:delete-item />
{/each}
