<script lang="ts">
    import "../app.css";

    let { children } = $props();
</script>

<svelte:head>
    <title>dinnerparty.js</title>
    <meta name="description" content="dinnerparty.js - come eat with us" />

    <meta property="og:title" content="dinnerparty.js" />
    <meta property="og:type" content="website" />
    <meta property="og:url" content="https://dinnerparty.dev" />
    <meta property="og:image" content="https://dinnerparty.dev/dinnerparty.js-link-preview.png" />
    <meta property="og:site_name" content="dinnerparty.js" />
    <meta property="og:description" content="dinnerparty.js - come eat with us" />

    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:title" content="dinnerparty.js" />
    <meta name="twitter:description" content="dinnerparty.js - come eat with us" />
    <meta name="twitter:image" content="https://dinnerparty.dev/dinnerparty.js-link-preview.png" />
    <meta name="twitter:site" content="@dinnerpartyjs" />
    <meta name="twitter:creator" content="@dinnerpartyjs" />
</svelte:head>

<div class="flex h-[100svh] w-screen flex-col bg-[#F2E7E3] lg:p-6">
    <div class="relative flex flex-1 flex-col lg:rounded-sm lg:border-2 lg:border-black">
        <header class="absolute top-0 z-50 w-full">
            <div class="flex items-center justify-between p-4 lg:px-6 lg:py-4">
                <div class="h-18 w-18 lg:h-20 lg:w-20">
                    <img
                        src="/dinnerparty.js-small.svg"
                        alt="dinnerparty.js logo"
                        class="h-full w-full object-contain"
                    />
                </div>
                <a
                    href="https://instagram.com/dinnerparty.js"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="h-8 w-8 lg:h-10 lg:w-10"
                    aria-label="Instagram"
                >
                    <img
                        src="/black-instagram-icon.svg"
                        alt="Instagram"
                        class="h-full w-full object-contain"
                    />
                </a>
            </div>
        </header>
        {@render children()}
    </div>
</div>
