<script></script>

<slot />

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/tippy.js@6.3.2/dist/tippy.css" />
</svelte:head>

<style lang="sass">
  @use '$src/vars'
  @use 'src/oc'

  :global(*)
    margin: 0
    padding: 0
    box-sizing: border-box

  :global(body)
    font-family: vars.$ff
    background: oc.$dark-8
    color: oc.$gray-5
    min-height: 100vh

  :global(svg)
    display: block
    user-select: none
    @include vars.transition(all)

  :global(body .tippy-box)
    background: oc.$dark-5
    font-size: 12px
    font-family: vars.$ff
    color: vars.$c-white
</style>
