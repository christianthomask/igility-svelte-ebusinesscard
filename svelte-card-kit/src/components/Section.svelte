<script>
    export let title;
    export let text;
    export let bgColor


</script>

<div class="{bgColor} backdrop-filter backdrop-blur-lg p-8 text-neutral-50 flex flex-col gap-1">
    <h2 class="text-xl leading-7 font-extrabold">{title}</h2>
    <p class="text-base leading-6 font-medium">{text}</p>
</div>
