<script lang="ts">
  import Portal from './Portal.svelte';
</script>

<p>Test Test Test Test Test Test Test Test Test Test</p>
<p>Test Test Test Test Test Test Test Test Test Test</p>
<p>Test Test Test Test Test Test Test Test Test Test</p>
<p>Test Test Test Test Test Test Test Test Test Test</p>
<p>Test Test Test Test Test Test Test Test Test Test</p>

<Portal>
  <div style="background: blue; padding:10px; position:fixed; top:0; ">
    <button on:click={() => console.log('It works!')}
      >Should cause a console message</button
    >
  </div>
</Portal>
