<script>
    export let category = '';
    export let title = '';
    export let image = '';
</script>

<section class="bg-white dark:bg-gray-900">
    <div class="container py-10 mx-auto">
        <section class="mt-8 space-y-8 lg:mt-12">
                <section class="lg:flex lg:items-center">
                    <div class="lg:w-1/2">
                        <p
                            class="text-lg tracking-wider text-blue-500 uppercase dark:text-blue-400"
                        >
                            {category}
                        </p>
                        <h2
                            class="mt-2 text-2xl font-semibold text-gray-800 capitalize dark:text-white"
                        >
                            {title}
                        </h2>
                    </div>

                    <div class="mt-4 lg:w-1/2 lg:mt-0">
                        <img
                            class="object-cover w-full h-64 rounded-lg md:h-96"
                            src={image}
                            alt=""
                        />
                    </div>
                </section>
        </section>
    </div>
</section>
