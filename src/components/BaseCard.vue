<template>
    <el-card class="box-card">
        <div v-if="" slot="header" class="clearFix">
            <span>卡片名称</span>
            <el-button style="float: right; padding: 3px 0" type="text">操作按钮</el-button>
        </div>
        <div class="text item">
            <slot></slot>
        </div>
    </el-card>
</template>

<script>
    export default {
        name: "BaseCard",
        props: {
            header: {},
            bodyStyle: {},
            shadow: {
                type: String
            }
        }
    }
</script>

<style scoped>
    .text {
        font-size: 14px;
    }

    .item {
        margin-bottom: 18px;
    }

    .clearFix:before,
    .clearFix:after {
        display: table;
        content: "";
    }
    .clearFix:after {
        clear: both
    }

    .box-card {
        width: 100vm;
    }
</style>
