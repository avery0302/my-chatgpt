<template>
    <div class="container">
        <div class="bg left">
            <div class="bg-yellow favicon">111</div>
            <div class="bg-blue feature">222</div>
            <div class="bg-green user">333</div>
        </div>
        <div class="right">
            <div class="bg-yellow header">222</div>
            <div class="bg-blue chat">333</div>
        </div>
    </div>
</template>

<script setup>
</script>

<style scoped>
.container {
    display: flex;
    height: 100%;

    .left {
        width: 50px;

        .favicon {
            height: 50px
        }
    }

    .right {
        flex: 1;
        display: flex;
        flex-direction: column;

        .header {
            height: 50px;
        }

        .chat {
            flex: 1
        }
    }
}
</style>