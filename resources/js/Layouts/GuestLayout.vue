<script lang="ts" setup></script>

<template>
    <div
        class="flex min-h-screen flex-col items-center bg-gray-50 sm:justify-center sm:pt-0 dark:bg-gray-900"
    >
        <div
            class="container w-full overflow-hidden bg-white shadow-md sm:rounded-lg dark:bg-gray-800"
        >
            <slot/>
        </div>
    </div>
</template>
