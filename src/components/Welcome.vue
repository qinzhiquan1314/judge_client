<template>
    <div>
        <h3>welcome</h3>
        <h3>作者正在找工作，欢迎联系</h3>
        <button @click.prevent="support_DialogVisible=true">联系作者</button>

        <el-dialog
                title="联系"
                :visible.sync="support_DialogVisible"
                width="90%">
            <el-collapse>
                <el-collapse-item title="联系作者" name="1">
                    <h5>作者正在找工作，欢迎联系^_^</h5>
                    <table>
                        <thead>
                        <tr>
                            <td><el-tag>QQ:1643711109</el-tag></td>
                            <td><el-tag>微信:1643711109</el-tag></td>
                        </tr>
                        </thead>
                        <tbody>
                        <tr>
                            <td><img src="../assets/qq.jpg"></td>
                            <td><img src="../assets/vx.png"></td>
                        </tr>
                        </tbody>
                    </table>

                    <el-tag>手机:15078552193</el-tag>
                </el-collapse-item>
            </el-collapse>
            <el-collapse>
                <el-collapse-item title="支持作者" name="2">
                    <table>
                        <thead>
                        <tr>
                            <td><el-tag>QQ</el-tag></td>
                            <td><el-tag>微信</el-tag></td>
                            <td><el-tag>支付宝</el-tag></td>
                        </tr>
                        </thead>
                        <tbody>
                        <tr>
                            <td><img src="../assets/qq2.jpg"></td>
                            <td><img src="../assets/vx2.jpg"></td>
                            <td><img src="../assets/my.jpg"></td>
                        </tr>
                        </tbody>
                    </table>
                </el-collapse-item>
            </el-collapse>
        </el-dialog>
    </div>
</template>

<script>
    export default {
        name: "Welcome",
        data(){
            return {
                support_DialogVisible:false,//支持
            }
        },
        methods:{

        }
    }
</script>

<style scoped>
    img{
        width:200px
    }
</style>