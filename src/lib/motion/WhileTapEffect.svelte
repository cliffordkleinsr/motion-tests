<script>
    import Box from "$lib/tags/Box.svelte";
    import { Motion } from "motion-start";
  </script>
  
  <Box cls="bg-slate-800 flex gap-3 md:gap-10 text-black">
    <Motion
      whileTap={{
        rotate: 45,
        scale: 0.75,
      }}
      let:motion><div class="box" use:motion>Rotate</div></Motion
    >
    <Motion
      whileTap={{
        scale: 0.84,
      }}
      let:motion><div class="box" use:motion>Simple</div></Motion
    >
  </Box>
  