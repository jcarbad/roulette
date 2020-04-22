<template>
    <div :class="[`text-center w-12 py-2`, color == 'red' ? 'bg-red-600 text-gray-700' : 'bg-gray-800 text-white']">
        <slot></slot>
    </div>
</template>

<script>
export default {
    name: 'Cell',
    props: {
        color: {
            type: String,
            required: true
        }
    }
}
</script>