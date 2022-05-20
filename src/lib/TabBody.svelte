
<script lang="ts">

    export let selectedContent: number = 0;
    const content = ['Texto do primeiro tab',
                     'Texto do segundo tab', 
                     'Texto do terceiro tab', 
                     'Texto do quarto tab'];


</script>

<div class='tab-container'>
    {content[selectedContent]}   
    
</div>

<style>
    .tab-container {
    width: 514px;
    height: 130px;
    left: 52px;
    top: 109px;

    font-family: Arial, Helvetica, sans-serif;
    font-style: normal;
    font-size: 20px;
    background: #F0F0F0;
    border: 1px solid #AAAAAA;
    box-sizing: border-box;
    border-radius: 10px;
    padding: 26px 23px;
}
</style>