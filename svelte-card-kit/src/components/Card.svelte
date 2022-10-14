<script>
    export let title;
    export let text;
    export let ctaText;
    export let ctaLink
    export let bgColor;
    export let classes;

</script>

<div class="w-full h-fit px-4 flex justify-center">
    <div class="{bgColor} backdrop-filter backdrop-blur-lg rounded-lg p-4 text-neutral-50 flex flex-col gap-2 {classes}">
        <h2 class="text-xl leading-7 font-extrabold">{title}</h2>
        <p class="text-base leading-6 font-medium">{text}</p>
        <div class="w-full flex justify-center">
            <a href="{ctaLink}" class="px-3 py-2 bg-blue-700 rounded-lg">
                <span class="text-lg leading-7 font-extrabold">
                    {ctaText}
                </span>
            </a>
        </div>
    </div>
</div>