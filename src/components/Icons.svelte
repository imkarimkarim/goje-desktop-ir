<script>
  import {
    MonitorIcon,
    CheckIcon,
    ToolIcon,
    FileTextIcon,
    DatabaseIcon,
  } from "svelte-feather-icons";
  export let name;
  const size = "40";
</script>

<div>
  {#if name === "monitor"}
    <MonitorIcon {size} />
  {:else if name === "check"}
    <CheckIcon {size} />
  {:else if name === "tool"}
    <ToolIcon {size} />
  {:else if name === "pdf"}
    <FileTextIcon {size} />
  {:else if name === "database"}
    <DatabaseIcon {size} />
  {/if}
</div>
