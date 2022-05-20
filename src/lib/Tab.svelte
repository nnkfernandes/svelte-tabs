<script lang="ts">
    
    import TabBody from "./TabBody.svelte";
    import TabButton from "./TabButton.svelte";
    
    const names = ['Tab 1', 'Tab 2', 'Tab 3', 'Tab 4']; 

    let tabIndex = 0;

    function handleClick(i: number){
        tabIndex = i;

    }
    

</script>


<div class='wrapper'>
    <div class='btn-wrapper'>
        {#each names as name, i}
           <TabButton onClick={() => handleClick(i)}>{name}</TabButton>
        {/each}
    </div>

    <TabBody selectedContent={tabIndex}/>
</div>


<style>

.wrapper {
    display: flex;
    width: 100%;
    height: 100vh;
    justify-content: center;
    align-items: center;
    flex-flow: column;
}

.btn-wrapper {
    width: 514px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 19px;
}
</style>